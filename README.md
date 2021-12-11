# Museo de pokemones
En esta oportunidad para nuestro proyecto de Ursina hicimos un museo
de pokemones , donde la persona que ejecute el programa podra ver 
el museo y los pokemones pixeleados.

* Para hacer el piso del museo utilizamos las siguientes lineas 
de código:

      platform = Entity(model="plane", collider="mesh",texture="piso", scale=(250,250,300), position=(0,-11,0))

* Para hacer el museo importamos lo siguiente:

      from ursina import *
      from ursina.prefabs.first_person_controller import FirstPersonController

      app = Ursina()
      player = FirstPersonController(speed=30,position=(10,9, 0))

* Para hacer las paredes y el techo:
  
      Entity(model="cube", collider="mesh",texture="pared",scale=250,position=(250,0,0))
      Entity(model="cube", collider="mesh",texture="pared",scale=250,position=(0,250,0))
      Entity(model="cube", collider="mesh",texture="pared",scale=250,position=(-250,0,0))
      Entity(model="cube", collider="mesh",texture="pared",scale=250,position=(0,0,250))

* Cartas para la pared del frente (escala largo,ancho y fondo):

      Entity(model="cube", scale=(40,50,1), collider="mesh",texture="cartaCHARMENDAR",position=(77,20,120))
      Entity(model="cube", scale=(40,50,1), collider="mesh",texture="cartaPIKACHU",position=(10,20,120))
      Entity(model="cube", scale=(40,50,1), collider="mesh",texture="cartaESCUAROL",position=(-50,20,120))

* Cartas para la pared derecha (escala largo,ancho y fondo):

      Entity(model="cube", scale=(1,60,40), collider="mesh",texture="cartaGIBLE",position=(120,30,-100))
      Entity(model="cube", scale=(1,60,40), collider="mesh",texture="cartaAMONGUS",position=(120,30,-50))
      Entity(model="cube", scale=(1,60,40), collider="mesh",texture="cartaCHIKORITA",position=(120,30,0))
      Entity(model="cube", scale=(1,60,40), collider="mesh",texture="cartaGARCHOMP",position=(120,30,50))
      Entity(model="cube", scale=(1,60,40), collider="mesh",texture="cartaMEW",position=(120,30,100))

* Cartas para la pared de la izquierda:

      Entity(model="cube", scale=(1,60,40), collider="mesh",texture="cartaIVI",position=(-120,30,-100))
      Entity(model="cube", scale=(1,60,40), collider="mesh",texture="cartaPIPLUT",position=(-120,30,-50))
      Entity(model="cube", scale=(1,60,40), collider="mesh",texture="cartaROSELIA",position=(-120,30,0))
      Entity(model="cube", scale=(1,60,40), collider="mesh",texture="cartaABSOL",position=(-120,30,50))
      Entity(model="cube", scale=(1,60,40), collider="mesh",texture="cartaRIOLU",position=(-120,30,100))

* Para hacer la función para salir del juego:

      def input(key):
        if key == 'escape':
            quit()

* Para el cielo:
     
      Sky()

* Para la puerta del museo:

      Entity(model="puerta.obj", scale=(2.5,2.5,0.5), collider="mesh",color = color.black,position=(1,-20,-135))


