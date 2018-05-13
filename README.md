## Ambiente de desenvolvimento

Um ambiente de desenvolvimento corretamente configurado é um item imprescindível no dia a dia de um programador. 

Vamos agora falar sobre o `vagrant`, um dos ambientes mais utilizados pelos devs php hoje em dia.

O vagrant tem como princípio criar máquinas virtuais de forma dinâmica, através de comandos simples via shell e/ou arquivos de configuração personalizados.

Em determinados cenários, você precisa que seu ambiente de desenvolvimento seja uma cópia real do que é o ambiente de homolog/prod, e o vagrant vem para suprir essa necessidade.

Você consegue uma réplica exata dos ambientes acima mencionados na questão de pacotes, versão do OS e ate estrutura de diretórios. 

Outro benefício é o fato de que o programador pode estar em um SO windows usando um servidor linux, eliminando a necessidade de instalação do PHP, MySQL, Vagrant, etc no host.

O Vagrant trabalha em cima do virtualbox ou do vmware, duas soluções bem conhe
cidas quando falamos sobre virtualização. Elas consistem no conceito de host/guest, onde nosso SO (que vamos chamar de `host`) pode ter inúmeras `boxes` com SOs separados, seus `kernels` e suas particularidades (onde vamos chamar de `guests`).

O Vagrant permite que a gestão dessas `boxes` sejam feitas via linha de comando, sem a necessidade de acessar o `guest` via interface do VirtualBox/Vmware.

Podemos trabalhar com o vagrant de duas formas: 

1 – Modo puro, com um script simples de criação da VM e a instalação manual dos pacotes.

2 – Com um orquestrador, como o Ansible ou o Puppet.

### Instalação

Para efetuar a instalação do Vagrant, é necessário antes que o VirtualBox ou o VMWare estejam corretamente instalados. 

Por ora, vamos trabalhar com o virtualbox pois é gratuito e de fácil configuração. É um pouco mais lento que o VMware, mas não existe prejuízo em performance.
Para tanto, siga as instruções de instalação para seu SO em https://www.oracle.com/br/virtualization/virtualbox/index.html . 

Em seguida, instale o Vagrant seguindo as instruções em https://www.vagrantup.com. 

A instalação de ambos os aplicativos é bem tranquila e não possui muitos problemas, tanto no Windows quanto no Linux. Apenas fique atento para habilitar a Virtualização de Hardware em sua BIOS para permitir que `boxes` 64-bit possam ser instaladas.


### Modo 'puro'

