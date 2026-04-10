# MD-Flash-Cart-4MB

Cartucho regravável simples para Mega Drive/Genesis com capacidade máxima de **4MB (32Mbit)**, totalmente compatível com o programador **FlashKit MD**.

![MDFC4MB-github](https://user-images.githubusercontent.com/24475390/149984222-c1a1d27c-d783-4d6d-8eb3-69ddee26fa4a.jpg)

---

## 📦 Sobre o projeto

Este é um projeto de placa de circuito impresso (PCB) desenvolvido em **KiCad**, já incluindo os arquivos **Gerber prontos para fabricação**.

O objetivo é permitir a construção de um cartucho funcional para o **:contentReference[oaicite:0]{index=0} / Genesis**, utilizando uma solução simples e eficiente com o mínimo de componentes necessários.

A memória utilizada é:

- **MXIC MX29L3211** (principal)
- Compatível também com **MX29LV320**

Encapsulamento: **(P)SOP-44**

![MDFC4MB-PCB-github](https://user-images.githubusercontent.com/24475390/150021381-3bffb65b-c416-45cf-a307-c182a318816e.jpg)

---

## 🔧 Componentes necessários

Para montagem do cartucho são necessários apenas:

- 1x Memória Flash (MX29L3211 ou MX29LV320)
- 1x Regulador de tensão **AMS1117 3.3V** (SOT-223)
- 1x Capacitor cerâmico **100nF (104)**

O capacitor é importante para garantir a estabilidade do funcionamento no console (não é obrigatório para gravação).

---

## 💡 Alternativa com LED

O regulador de tensão pode ser substituído por um **LED SMD**:

- Deve ser soldado entre entrada e saída (ânodo/cátodo corretamente posicionados)
- O LED atua como queda de tensão (~1.6V)
- Como bônus, funciona como indicador de atividade do cartucho

⚠️ Atenção:
- LEDs de cores diferentes possuem quedas de tensão diferentes  
- LED **laranja** apresentou melhor resultado  
- LED **azul** pode reduzir tensão excessivamente  

---

## ⚡ Compatibilidade elétrica

- A memória (CMOS 3.3V) é compatível com a lógica TTL 5V do console
- Não é necessário uso de resistores nas linhas de sinal (diferente de outros projetos)

---

## 🎮 Compatibilidade com 32X

O cartucho é compatível com o acessório **32X**, já que a velocidade de leitura das memórias flash modernas é suficiente para atender à demanda.

---

## 💾 Gravação

Para gravação do cartucho é necessário:

👉 **FlashKit MD**  
👉 Software: [FlashKit MD Plus](https://github.com/MiGeRA/FlashKit-MD-Plus)

Versões recomendadas:

- **v1.0.2.0** → suporte ao MX29L3211 (~150s para gravação completa)
- **v1.0.3.0** → suporte ao MX29LV320 (~100s, mais rápido)

---

## 💰 Custo-benefício

Este projeto apresenta excelente custo:

- ~3x mais barato que soluções comerciais (ex: Krikzz)
- ~2x mais barato que clones disponíveis (ex: KY-tech)

Além disso:

- Encapsulamento SOP-44 facilita a soldagem
- PCB com máscara branca proporciona acabamento visual mais profissional

---

## ⚠️ Observações

- Capacidade máxima: **4MB**
- Apenas um jogo por gravação
- Requer programador compatível

---

## 📜 Licença

Copyright: MiGeRA (aka Th.K)

Este projeto é Open Hardware e está licenciado sob a:

**CERN Open Hardware License v1.2**

Você pode utilizar, modificar e redistribuir conforme os termos da licença:

http://ohwr.org/cernohl

⚠️ Este projeto é fornecido **sem garantias**, incluindo comercialização ou adequação a qualquer finalidade específica.
