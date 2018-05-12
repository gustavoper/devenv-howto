## Ambiente de desenvolvimento

Um ambiente de desenvolvimento corretamente configurado é um item imprescindivel no dia-a-dia de um programador. 

Vamos agora falar sobre o `vagrant`, um dos ambientes mais utilizados pelos devs php hoje em dia.

O vagrant tem como principio criar máquinas virtuais de forma dinamica, atraves de comandos simples via shell e arquivos de configuração personalizados.

Em determinados cenarios, voce precisa que seu ambiente de desenvolvimento seja uma copia real do que é o ambiente de homolog/prod, e o vagrant vem para suprir essa necessidade.

Voce consegue uma replica exata dos ambientes acima mencionados na questao de pacotes, versao do OS e ate estrutura de diretorios. 

Outro beneficio é em casos especificos onde um servidor não pode ter o luxo de pacotes atualizados ou ainda obter pacotes de fontes de terceiros.  


O Vagrant trabalha em cima do virtualbox ou do vmware, que são duas soluções para virtualização.



Por ora, vamos trabalhar com o virtualbox pois é gratuito e de facil configuração. É um pouco mais lento que o VMware, mas não existe prejuizo em performance.

Podemos trabalhar com o vagrant de duas formas: 


1 - Modo puro, com um script simples de criação da VM e a instalação manual dos pacotes.


2 - Com um orquestrador, como o Ansible ou o Puppet.



