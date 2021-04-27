//função = function , return retornar valor

    function MultiplicarPorDois(valor){
        return valor* 2;

    }

console.log(MultiplicarPorDois(5));


// console.log 

let nome = ('lucas')

console.log(nome);

//Operadores Aritimeticos(Matematicos)
//Operadores Atribuição
//Operadores de Comparação
//Operadores Lógico
//Operadores Bitwise

//Operadores Aritiméticos
let salario = 100;

// = , - ,* , / , **

// -- ++ incremento
console.log(salario + salario);

//++ -- 
let idade = 18;
console.log(++idade);
console.log(idade)


//Operadores de Atribuição (= , += , -=)
let valorTecladoGamer = 100;
// valorTecladoGamer = valorTecladoGamer + valorTecladoGamer  
valorTecladoGamer -= valorTecladoGamer
console.log(valorTecladoGamer)

//Operadores de igualdade
//igualdade escrita obs: comparação de valor
console.log ( 1 === 1 );
console.log('1' === 1 );


//Operador Ternario
// Tenho um cliente e se esse cliente tiver pontos,100 premium, comum
let pontos = 200;
let tipo = pontos > 100 ? 'premium' : 'comum'
console.log(tipo);

// Operadores Lógicos

// Operadores logicos e (e&& ,ou|| ,nao NOT)
// Retorna TRUE se os dois opereradores forem TRUE

//operador &&
//console.log(false && false);
//console.log(true && true);

let maiorDeIdade = false;
let possuiCarteiraDeTrabalho = true;
let podeAplicar = maiorDeIdade && possuiCarteiraDeTrabalho;

console.log('pode aplicar', podeAplicar);


//Operador logico not (!)

let candidatoRecusado = !podeAplicar;

console.log('Candidato recusado', candidatoRecusado);




let corPersonalizada = '';
let corPadrao = 'azul';
let corPerfil = corPersonalizada || corPadrao;

console.log(corPerfil);

//falsy
//underfined
//null
//e
//false
// ''
// NaN - not e number

//Trunthy
//
 
let a = 'azul';
let b = 'verde';

let c = a;

console.log(a);
console.log(b);

// if else
// switch .. case

// Se a hora estiver entr 6:00 até 12:00 : Bom dia!
// Se estiver entre 12:00 até 10:00 : Boa tarde!
// Caso contrario : Bom dia!

//if(condição){
    // codico a ser axecutado
// }
// else if (outraCondição){
     // codico a ser executado
// }
//else {
    // condição a ser executado
//  }

let hora = 22
if(hora > 6 && hora <12 ){
     console.log('Bom dia!'); 
 }
 else if (hora > 12 && hora < 18){
     console.log('Boa tarde');
  }
else {
    console.log('Boa noite');
}


//swich .. case

let permissao; // comum,gerente,diretor...
permissao = 'comum';
switch(permissao) {
    case 'comum':
    console.log('usuario comum');
    break;
     
    
    case 'gerente':
    console.log('usuario gerente');
    break;
    

    case 'cdiretor':
    console.log('usuario diretor');
    break;

   default:
    console.log('usuario nao reconhecido')
}

// 1 FOR  2 WILE 3 DO.WILE 4 FOR.IN 5 FOR.OF

// FOR 

    for(let i = 0; i < 5; i++) {
    console.log('madaleno',i);
}
 
//for in 

const pessoa = {
    nome: 'lucas',
    idade: 25

};

    for(let chave in pessoa){
console.log(chave,pessoa)

    }

const cores = ['vermelho', 'azul']
for (let indice in cores) {
 console.log(indice,cores[indice])
    }


//for off
for(let cor of cores){
    console.log(cor)
}

// fizz buzz
    const resultado = fizzBuzz(6);
    console.log(resultado);
   
    function fizzBuzz(entrada){
        if (typeof entrada !== 'number')
   
        return'Não é um numero';
        if ((entrada % 3 === 0) && (entrada % 5 === 0 ))
            return "FizzBuzz";
        if (entrada % 3 === 0)
            return 'Fizz';
        if (entrada % 5 ===0)
            return 'Buzz';
        return(entrada);
    }
// vereficar ponto
// velocidade maxima ate 100
// a cada 5km acima limite voçe ganha 1 ponto
//math.florr
// caso pontos maior que 12 => 'Carteira suspensa'

vereficarVelocidade(130);
function vereficarVelocidade(velocidade) {
   const velocidadeMaxima = 70;
    const kmPorPonto = 5;
    if(velocidade <= velocidadeMaxima)
    console.log('ok');
    else {
        const pontos = Math.floor(((velocidade - velocidadeMaxima) / kmPorPonto));
        
        if (pontos >= 12)
         console.log('carteira suspensa');
         else
         console.log('Pontos',pontos);
    }

}

exebirTipo(5);
function exebirTipo(limite) {
    for (let i = 0; i <= limite; i++) {
        if (i % 2 === 0)
         console.log(i,'par');
        else 
        console.log(i,'impar');
    }
    }

