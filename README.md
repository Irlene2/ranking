# ranking
calculadora de saldo
function calcularSaldo(vitorias, derrotas) {
  // Calcula o saldo de vitórias
  let saldoVitorias = vitorias - derrotas;

  // Usa uma estrutura de decisão para determinar o nível
  let nivel = "Ferro";
  if (saldoVitorias < 10) {
    nivel = "Ferro";
  } else if (saldoVitorias < 20) {
    nivel = "Bronze";
  } else if (saldoVitorias < 50) {
    nivel = "Prata";
  } else if (saldoVitorias < 80) {
    nivel = "Ouro";
  } else if (saldoVitorias < 90) {
    nivel = "Diamante";
  } else if (saldoVitorias < 100) {
    nivel = "Lendário";
  } else {
    nivel = "Imortal";
  }

  // Retorna o saldo de vitórias
  return saldoVitorias;
}

// Declara as variáveis
let vitorias = 10;
let derrotas = 5;

// Chama a função
let saldoVitorias = calcularSaldo(vitorias, derrotas);

// Exibe a mensagem
console.log(`O Herói tem de saldo de **${saldoVitorias}** está no nível de **${nivel}**`);
vitorias = 10;
derrotas = 5;

saldoVitorias = calcularSaldo(vitorias, derrotas);

console.log(`O Herói tem de saldo de **${saldoVitorias}** está no nível de **${nivel}**`);

