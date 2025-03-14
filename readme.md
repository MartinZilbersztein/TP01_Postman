# TP 01 - Postman
#### Docente: Jesica Rodríguez
#### Alumno: Martín Zilbersztein

El objetivo de este trabajo es comenzar a aprender los conceptos básicos de Postman, analizar archivos JSON y poder hacer uso de las APIs.

APIs utilizadas:
* [OMDbAPI](http://omdbapi.com/)
* [PokeAPI](https://pokeapi.co/)

#### Parte 1: OMDb
1. Consulta N°1: Identificar cuántos títulos de películas incluyen la palabra "Cars".
    <br>
    Comando empleado:
    ```
    http://www.omdbapi.com/?apikey=9d230b0c&s=cars
    ```
    Al utilizar el parámetro "s" se listan todos los datos de cada película cuyo nombre incluya "cars". <br>
    Al final del response, se obtiene la cantidad de resultados.<br>
    ![Imagen de la primera consigna](/images/Primera%20screenshot.png) <br>
    Por lo tanto, la respuesta a la primera consulta es <b>376</b>.
    
2. Consulta N°2: Buscar "Hunger" y devolver el nombre de la última película que retorna OMDb API
<br>
Comando empleado:
    ```
    http://www.omdbapi.com/?apikey=9d230b0c&t=Hunger
    ```
    Al utilizar el parámetro "s" se listan todos los datos de cada película cuyo nombre incluya "Hunger", y se elige la última que tenga como título precisamente lo buscado. <br>
    ![Imagen de la primera consigna](/images/tercera%20screenshot.png)
    
3. Consulta N°3: Obtener de la película "Monsters, Inc." la cantidad de votos de imdb, qué actores actuaron y ver el Poster (en una nueva página). <br>
Comando empleado:
    ```
    http://www.omdbapi.com/?apikey=9d230b0c&t=Monsters, Inc.
    ```
    <br>
    Esto devuelve la información de la única película cuyo título coincida exactamente con el parámetro enviado.
    ![Imagen de la segunda consigna](/images/segundascreenshot.png)<br>
    ![Imagen de la segunda consigna 2](/images/cuartascreenshot.png)<br>
    ![Imagen de la segunda consigna 3](/images/quintascreenshot.png)
    <br>
    Por lo tanto, <b>la cantidad de votos es de 1.017.055 y los actores son Billy Crystal, John Goodman y Mary Gibbs.</b> <br>
    P.D.: es posible que no se puedan visualizar las imágenes. Esto ya ha sido hablado previamente durante clase.
<br>
4. Consulta N°4: Obtener de la película "Rocky IV" su género, director y cuántos minutos de duración tiene la película.
<br>
Comando empleado:
    ```
    http://www.omdbapi.com/?apikey=9d230b0c&t=Rocky IV
    ```
    <br>
    Este envía un request a la API y devuelve en pantalla datos relacionados a la película llamada "Rocky IV".<br>
    ![Imagen de la segunda consigna](/images/sextascreenshot.png)<br>
    ![Imagen de la segunda consigna 4](/images/septimascreenshot.png)<br>
    ![Imagen de la segunda consigna 5](/images/octavascreenshot.png)
    <br>
    Por lo tanto, <b>la película "Rocky IV" pertenece a los géneros drama y deportes, su director es Sylvester Stallone y alberga una duración de 91 minutos.</b>

5. Consulta N°5: Obtener de la película cuyo imdbID es "tt0067992" su título y el año en el que se estrenó.
<br>
Comando empleado:<br>
    ```
    http://www.omdbapi.com/?apikey=9d230b0c&i=tt0067992
    ```
    <br>
    De esta forma, se obtiene toda la información de la película cuyo ID es el mencionado en el enunciado.
    <br>
    ![Imagen consulta 5](/images/quintascreenshot.png) <br>
    ![Imagen consulta 6](/images/decimascreenshot.png)<br>
    Por lo tanto, el título de la película es <b>Willy Wonka & the Chocolate Factory</b> y el año en el que se estrenó es <b>1971</b>

#### Parte 2: PokeAPI
1. Consulta N°1: Obtener la información completa del pokémon llamado Pikachu.<br>
    Comando empleado:<br>
    ```
    https://pokeapi.co/api/v2/pokemon/pikachu
    ```
    De esta forma, la API devuelve toda la información del pokémon cuyo nombre es "Pikachu". <br>
    Se adjunta un recorte de la información visible en pantalla tras la utilización del comando.
    ![Imagen PokeApi](/images/decimoprimerascreenshot.png)

2. Consulta N°2: Consultar cuántos tipos de Pokémon diferentes existen en la API.<br>
Comando empleado:<br>
    ```
    https://pokeapi.co/api/v2/pokemon
    ```
    Este envía una solicitud de una lista de todos los pokémons existentes, incluyendo sus nombres y las instrucciones para solicitar información sobre uno específico.
    <br> 
    ![Imagen PokeApi 2](/images/decimosegundascreenshot.png)
    <br>
    Por tanto, la cantidad de pokémons registrados en la API es de <b>1302</b>.

3. Consulta N°3: Obtener el nombre del Pokémon cuyo ID es 150.<br>
Comando empleado:<br>
    ```
    https://pokeapi.co/api/v2/pokemon/150
    ```
    Este solicita toda información relacionada al pokémon cuya ID es 150.
    <br>
    ![Imagen PokeApi 3](/images/decimotercerascreenshot.png)
    <br>
    Por tanto, el nombre del pokémon cuya ID es 150 es <b>Mewtwo</b>.

4. Consulta N°4: Buscar los movimientos que puede aprender el Pokémon Charizard.<br>
Comando empleado:<br>
    ```
    https://pokeapi.co/api/v2/pokemon/charizard
    ```
    Este solicita la información relacionada al pokémon denominado Charizard.<br>
    ![Imagen PokeApi 4](/images/decimocuartascreenshot.png)
    <br>
    Por lo tanto, las habilidades que el pokémon Charizard puede aprender son las <b>llamaradas</b> y el <b>poder solar</b>
    
5. Consulta N°5: Obtener la altura y peso del Pokémon Bulbasaur<br>
Comando empleado:<br>
    ```
    https://pokeapi.co/api/v2/pokemon/charizard
    ```
    Este solicita la información relacionada al pokémon denominado Bulbasaur.<br>
    ![Imagen PokeApi 5](/images/decimoquintascreenshot.png)
    <br>
    ![Imagen PokeApi 6](/images/decimosextascreenshot.png)
    <br>
    Por lo tanto, el peso de Bulbasaur es de <b>69</b>, y su altura de <b>7</b>.


    

