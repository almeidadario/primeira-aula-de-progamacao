# primeira-aula-de-progamacao
joguinho matematico, criado com um codigo de progamacao
  
let acumuladordorDePontos = 0;
let chances = 3

while (chances > 0) {
  let numero1 = Math.floor(Math.abs(Math.random() * (100 - 0) + 0));
  let numero2 = Math.floor(Math.abs(Math.random() * (100 - 0) + 0));

  let valorDigitado = prompt("Quanto é " + numero1 + "+" + numero2 + "?");

  if (valorDigitado == (numero1 + numero2)) {
    acumuladordepontos = acumuladordorDePontos +5;
  } else if(valorDigitado != (numero1 + numero2)) {
    chances -=1;
    alert("quantidade de vidas = "+ chances);
  } 
}

alert("voce fez " + acumuladordorDePontos + " pontos!");
