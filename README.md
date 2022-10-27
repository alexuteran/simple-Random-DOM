# Ejemplo de Calculo de Numeros aleatorios, ambos incluidos, con las funciones
# Math.random y Math.floor, todo manipulado con el DOM


````````````JS````````````````````````
let boton = document.querySelector(".boton");
  
  function getRandom(min, max) {
  return Math.floor(Math.random() * (max - min + 1) + min);
}

boton.addEventListener("click", () => {
  let min = document.querySelector(".min").value;
  let max = document.querySelector(".max").value;
  document.querySelector(".numbero").innerHTML=getRandom(parseInt(min), parseInt(max));
 
});
