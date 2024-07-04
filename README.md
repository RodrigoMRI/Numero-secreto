
//Variables 
let numeroMaximo = 100
let numeroSecreto = Math.floor(Math.random()*numeroMaximo)+1;
let numeroUsuario = 0;
let intentos = 1;
//let palabraVeces = "vez";
let maximosIntentos = 3;

while (numeroUsuario != numeroSecreto) {
    numeroUsuario = parseInt(prompt(`Dime un número entre 1 y ${numeroMaximo}, por favor`));

    console.log(typeof(numeroUsuario));

    
    //Este codigo realiza 
    //la comparacion 
    

    if (numeroUsuario == numeroSecreto) {
        alert (`Acertaste el número, es: ${numeroUsuario}. Lo hiciste en ${intentos} ${intentos == 1 ? "juego" : "juegos"}.`);
    } else {
        if (numeroUsuario > numeroSecreto){
            alert ("El número secreto es menor");
        } else {
            alert ("El número secreto es mayor");
        }

           // intentos = intentos + 1
           intentos++; 
           //palabraVeces = "veces"  
        

        if (intentos > maximosIntentos) {
            alert (`Llegaste al número máximo de ${maximosIntentos} intentos`);
            break;
        }

    
        
        // incremento de contador cuando no se acierta

        //La condicion no se cumplio
        // alert ("Lo siento, no acertaste");
    }
        
} 

