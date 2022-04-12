# Projeto Loteca
Este é um projeto de simulador de loteria, onde o usuário digita 6 números e realiza um sorteio de outros 6 números, logo é verificado quantos números ele acertou.

## Tecnologia utilizadas
- *HTML*: Estrutura do site
- _CSS_: Estilização do site
- JS: Funções o site
- ~BootStrap~: Não foi utilizado

### Melhorias Possíveis
1. [ ] Subir para o GitHubPages
2. [ ] Alterar os alerts
3. [ ] Utilizar o Bootstrap
4. [ ] Deixar responsivo 

### Disponibilizado em
[GitHubPages](https://alexsouza-d.github.io/loteca/)

| ID | Primeira tela | Segunda Tela |
|----|---------------|--------------|
| 1 | Loteca Limpa   | loteca Preenchida |
| 2 | ![tela loteca não preenchida](![image](https://user-images.githubusercontent.com/68750695/162854852-ff9708dd-3ce5-498d-93d6-05c85afe7ae6.png)
) | ![loteca Preenchida](![image](https://user-images.githubusercontent.com/68750695/162854922-7792afd4-86a4-4a4c-8845-c011addad8c0.png)
) |

#### Função Principal
js:
function sorteio() {
  if(numEsco.length == 6){
  var cont = 0;
  numSort = [];

  while (cont < 6) {
    let num = Math.random() * 60;
    num = Math.ceil(num);
    if (!numSort.includes(num)) {
      numSort[cont] = num;
      console.log(numSort);
      cont++;
    }
  }
  
  document.getElementById("sorteados").innerHTML = numSort;
  contAcertos();
} else {
  alert("É necessario digitar seis numeros antes do sorteio")

}
}


#### comando git
Para iniciar o projeto

git init
 
