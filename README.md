# java-filme-
// Ação, ficção , aventura, comédia 

 // Homem de ferro, LIVRE, Ação, ficção 
// O rei leão , 12, ficção, aventura 
// Os vingadores, 13, ação, ficção 
// Carros, LIVRE,   ação, ficção, aventura
// Meu malvado favorito, 18, ação, comédia
// Toy story, LIVRE, comédia, ficção 
// Batman, 17, ação, ficção 

let campoIdade;

function setup() {
  createCanvas(400, 400);
  campoIdade = createInput("5");
}

function draw() {
  background(220);
  let idade = campoIdade.value();
  let recomendacao = geraRecomendacao(idade);
  text(recomendacao, width / 2, height / 2);
}

function geraRecomendacao(idade) {
  if(idade >= 10) {
    if(idade >= 14) {
      return "Toy story";
    } else {
      return "Homem de ferro";
    }
  } else {
    return "Batman ";
  }
}









