Projeto de automação residencial com Arduino, permitindo o controle de relés pela rede local ou até mesmo pela internet. Com ele, você pode controlar lâmpadas, eletrodomésticos ou outros equipamentos eletrônicos por meio de uma página web.

Materiais:

01 – Placa Uno R3
01 – Cabo USB
01 – Fonte DC Chaveada 9V 1A Plug P4
01 – Ethernet Shield W5100
01 – Cabo de Rede Conector RJ45 1,5m
xx – Jumpers Macho-Fêmea
01 – Módulo Relé 5v 2 Canais
01 – Fio Simples 1,0mm 3m
02 – Lâmpada E14 15W
02 – Soquete Lâmpada E14
01 – Plug Tomada Macho

O controle do módulo relé será feito pelas portas digitais 3 e 4 do Arduino, e a alimentação do módulo é feita pelo pino 5V. No circuito abaixo, utilizamos 2 lâmpadas ligadas à rede elétrica de 220V, portanto tome cuidado na hora de efetuar esse tipo de ligação, desligando o quadro geral de energia ou os disjuntores correspondentes ao circuito elétrico que você está utilizando.

Após a montagem do circuito, ligue o Ethernet Shield ao seu roteador utilizando um cabo de rede com conector RJ45.

A programação do Arduino utiliza a biblioteca Ethernet que já vem embutida na IDE do Arduino. Com ela, vamos criar um Web Server que vai receber as informações pela rede e acionar as portas  3 (relé 1) e 4 (relé 2).
No início do programa, altere as configurações de IP, default gateway e máscara de rede (linhas 15, 16 e 17) para que estejam adequadas à sua rede. O programa aguarda pela conexão do cliente (browser), e em seguida monta a página web com informações dos arquivos automacao_residencial.css e automacao_residencial.js, hospedados no servidor da FILIPEFLOP.

![automação-residencial-com-arduino-02.png](https://uploads.filipeflop.com/2015/11/automa%C3%A7%C3%A3o-residencial-com-arduino-02.png)

FONTE:www.filipeflop.com
