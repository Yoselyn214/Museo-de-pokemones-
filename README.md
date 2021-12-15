# _Museo de pokemones_
---------------------

🤓💻 En esta oportunidad para nuestro proyecto de Ursina hicimos un museo
de pokemones, donde la persona que ejecute el programa podra observar los pokemones que hemos realizado a base de pixeles  en el espacio que hemos creado, es decir, un museo virtual.


**🌈🙌Las artistas y fundadoras del museo "POKÉMON" son:**

      Miranda Chirinos, Yoselyn Victoria 
      Rojas Terrones, Janne Andrea 
      Merino Miranda, Lady Anallely
      Alvarez Flores, Irán María 

![Portada de Facebook 851x315 px](https://user-images.githubusercontent.com/91160075/145697622-8880c4c3-8c37-461f-afd1-ec83ad32b29a.gif)

* ✅ Para hacer el piso del museo utilizamos las siguientes lineas 
de código:

       platform = Entity(model="plane", collider="mesh",texture="piso", scale=(250,250,300), position=(0,-11,0))

* ✅ Para hacer el museo importamos lo siguiente:

      from ursina import *
      from ursina.prefabs.first_person_controller import FirstPersonController

      app = Ursina()
      player = FirstPersonController(speed=30,position=(10,9, 0))

* ✅ Para hacer las paredes y el techo:
  
      Entity(model="cube", collider="mesh", texture="pared", scale=250, position=(250,0,0))
      Entity(model="cube", collider="mesh", texture="pared", scale=250, position=(0,250,0))
      Entity(model="cube", collider="mesh", texture="pared", scale=250, position=(-250,0,0))
      Entity(model="cube", collider="mesh", texture="pared", scale=250, position=(0,0,250))
* ✅ Para hacer el título:
     ```
      Entity(model="cube", scale=(80,25,0) , collider="mesh",texture="titulo",position=(5,50,0))
     ```
* ✅ Cartas para la pared del frente (escala largo, ancho y fondo):

      Entity(model="cube", scale=(40,50,1), collider="mesh", texture="cartaCHARMENDAR", position=(77,20,120))
      Entity(model="cube", scale=(40,50,1), collider="mesh", texture="cartaPIKACHU", position=(10,20,120))
      Entity(model="cube", scale=(40,50,1), collider="mesh", texture="cartaESCUAROL", position=(-50,20,120))

* ✅ Cartas para la pared derecha (escala largo, ancho y fondo):

      Entity(model="cube", scale=(1,60,40), collider="mesh", texture="cartaGIBLE", position=(120,30,-100))
      Entity(model="cube", scale=(1,60,40), collider="mesh", texture="cartaAMONGUS", position=(120,30,-50))
      Entity(model="cube", scale=(1,60,40), collider="mesh", texture="cartaCHIKORITA", position=(120,30,0))
      Entity(model="cube", scale=(1,60,40), collider="mesh", texture="cartaGARCHOMP", position=(120,30,50))
      Entity(model="cube", scale=(1,60,40), collider="mesh", texture="cartaMEW", position=(120,30,100))

* ✅ Cartas para la pared de la izquierda:

      Entity(model="cube", scale=(1,60,40), collider="mesh", texture="cartaIVI", position=(-120,30,-100))
      Entity(model="cube", scale=(1,60,40), collider="mesh", texture="cartaPIPLUT", position=(-120,30,-50))
      Entity(model="cube", scale=(1,60,40), collider="mesh", texture="cartaROSELIA", position=(-120,30,0))
      Entity(model="cube", scale=(1,60,40), collider="mesh", texture="cartaABSOL", position=(-120,30,50))
      Entity(model="cube", scale=(1,60,40), collider="mesh", texture="cartaRIOLU",´position=(-120,30,100))
      
* ✅ Personajes y pokemones en 2-D:
     ```
      Entity(model="cube", scale=(15,25,0), collider="mesh", texture="Eevee", position=(50,0.5,60))
      Entity(model="cube", scale=(20,25,0), collider="mesh", texture="pokemon1", position=(-30,1,100))
      Entity(model="cube", scale=(20,25,0), collider="mesh", texture="pokemon2", position=(60,1,-85))
      Entity(model="cube", scale=(0,25,20), collider="mesh", texture="pokemon3", position=(90,1,-35))
      Entity(model="cube", scale=(0,25,20), collider="mesh", texture="pokemon4", position=(-70,1,-20))
      Entity(model="cube", scale=(0,25,20), collider="mesh", texture="pokemon5", position=(-80,1,20))
      Entity(model="cube", scale=(20,30,0), collider="mesh", texture="ash", position=(-70,4,80))
      Entity(model="cube", scale=(20,25,0), collider="mesh", texture="pokemon6", position=(15,-2,90))
      Entity(model="cube", scale=(0,25,20), collider="mesh", texture="pokemon7", position=(-90,1,70))
      Entity(model="cube", scale=(0,50,30), collider="mesh", texture="misty", position=(-90,13,-85))
      Entity(model="cube", scale=(0,35,25), collider="mesh", texture="pokemon8", position=(95,6,8))
      Entity(model="cube", scale=(20,25,0), collider="mesh", texture="pokemon9", position=(30,50,-20))
     ```

* ✅ Función para salir del juego:

      def input(key):
        if key == 'escape':
            quit()

* ✅ Para el cielo:
     
      Sky()

* ✅ Para la puerta del museo:

      Entity(model="puerta.obj", scale=(2.5,2.5,0.5), collider="mesh", color = color.black, position=(1,-20,-135))
      
 
* 💡 TIP:

  Para instalar la librería _FirstPersonController_ deberás copiar lo siguiente en tu editor favorito   
  ```
   from ursina.prefabs.first_person_controller import FirstPersonController
  ```
  Luego deberas seleccionar la linea de código anterior ya que probablemente aparezca subrayado en rojo. Solo selecciona la línea y aparecerá una bombilla roja, donde   deberás seleccionar ```install FirstPersonController packages ``` y esperar que se instale y listo ya podrás hacer un recorrido por nuestro museo de pokemones.
  
    
* 📂 *Las coordenadas de cada pokémon y personaje pixeleado han sido adjuntadas como archivos **.txt** en el README.md*


* 📸  Ahora le invitamos a un pequeño recorrido a nuestro museo por medio de una galería de fotos. ¡No se lo puede perder! 🤗









      
