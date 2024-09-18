## Botón guessSubmit no tiene función agregada
Se agrega función checkGuess() usando onclick

## se cambia formula para que el número random sea de 1 a 100
let randomNumber = Math.random() * 100;

## Se cambia el número de intentos de 5 a 10
  const ATTEMPS = 10;

## Se cambia intercambia condicionales ATTEMPS y randomNumber además de los colores del texto
if(userGuess === ATTEMPS) {
  lastResult.textContent = '!!!Perdistes!!!';
  lastResult.style.backgroundColor = 'red';
  lowOrHi.textContent = '';
  setGameOver();
} else if(guessCount === randomNumber) {
  lastResult.textContent = 'Felicitaciones! adivinaste el número!';
  lastResult.style.backgroundColor = 'black';
  setGameOver();
}
