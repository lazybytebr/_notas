# ✅ <span style="color: #fff; "> Projeto EstéticApp</span>

<!-- .slide: data-background-image="https://www.florence.edu.br/blog/wp-content/uploads/2021/04/Florence-profissional-de-Estetica.jpg" data-background-opacity="1" data-background-size="cover" data-background-repeat="no-repeat" -->

---

## Você fez a sua divulgação <br> Um cliente entrou em contato...

<!-- .slide: data-background-image="imagens/fundos/fundo01.jpg" data-background-opacity="1" data-background-size="cover" data-background-repeat="no-repeat" -->

<span style="width: 60%; display: block;">

"Gostaríamos de solicitar um orçamento para a criação de um sistema para nossa clínica de estética..."

</span>

<span style="position: absolute; top: 2rem; right: 0; width: 35%;">

![](https://png.pngtree.com/png-clipart/20230510/original/pngtree-sms-icon-dialog-chat-new-message-gmail-email-png-image_9154865.png)

</span>
--

## Por onde você começa? Quanto Cobraria?

<!-- .slide: data-background-image="imagens/fundos/fundo01.jpg" data-background-opacity="1" data-background-size="cover" data-background-repeat="no-repeat" -->

- Levantamento de Requisitos (Briefing)  <!-- .element: class="fragment" -->
- Modelagem do sistema ( UML - diagramas ) <!-- .element: class="fragment" -->
- Orçamento <!-- .element: class="fragment" -->
- Contrato <!-- .element: class="fragment" -->
- Entrada <!-- .element: class="fragment" -->
- Desenvolvimento <!-- .element: class="fragment" -->
- Testes/Homologação <!-- .element: class="fragment" -->

<span style="position: absolute; width: 35%; top: 5rem; right: 0;">

![](https://portalhospitaisbrasil.com.br/wp-content/uploads/checklist.jpg)

</span>

--

## Levantameno de Requisitos

<!-- .slide: data-background-image="imagens/fundos/fundo01.jpg" data-background-opacity="1" data-background-size="cover" data-background-repeat="no-repeat" -->

<span style="font-size: 1rem; width: 50%; display: inline-block; margin-top: 0; float: left;">
É o processo de descobrir, entender e documentar tudo o que o sistema precisa fazer para atender às necessidades dos usuários e do negócio.

- O que eles querem que o sistema faça (ex: cadastrar clientes, gerar relatórios, vender produtos online);

- Como eles esperam que isso funcione (ex: deve funcionar no celular, precisa ser rápido, seguro, etc.);

- Quais regras precisam ser seguidas (ex: só administradores podem apagar dados, cálculo de frete, etc.).

O objetivo é criar um documento claro que guie os desenvolvedores na criação do sistema certo, evitando erros, retrabalho e desperdício de tempo.
</span>
<span style="position: absolute; width: 35%; top: 5rem; right: 0;">
![](https://www.mendoncadev.com.br/images/articles/levantamento-de-requisitos-a-base-de-um-software-bem-sucedido.png)
</span>

---
<span style="position: relative; float: left; margin-top: 12rem;" >

## Briefing <br> [link](https://docs.google.com/document/d/1LgUFeGdYu9DxBxyoPS-VqlqhthEhNGp_5VpvMtmWSFw/edit?usp=drive_link)

<!-- .slide: data-background-image="imagens/fundos/fundo01.jpg" data-background-opacity="1" data-background-size="cover" data-background-repeat="no-repeat" -->

</span>

<span style="position: absolute; top: 4rem; right: 0;" >
    <iframe src="https://drive.google.com/file/d/1LgUFeGdYu9DxBxyoPS-VqlqhthEhNGp_5VpvMtmWSFw/preview" 
        width="800" height="700" allow="autoplay"></iframe>
</span>

---
## UML

<span style="font-size: 1rem; width: 50%; display: inline-block; margin-top: 0; float: left;">

UML (Unified Modeling Language) é uma linguagem visual padronizada usada para planejar, visualizar, construir e documentar sistemas de software. 

Em vez de escrever código diretamente, usamos diagramas para representar ideias, fluxos, estruturas e comportamentos do sistema antes de implementá-lo.

Ela ajuda desenvolvedores, analistas e clientes a entenderem melhor como o sistema funciona ou deve funcionar, mesmo sem saber programar.

</span>

<span style="position: absolute; width: 35%; top: 5rem; right: 0;">

![](http://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/UML_logo.svg/640px-UML_logo.svg.png)

</span>

--
## Diagrama de Caso de Uso

<span style="position: absolute; width: 60%; top: 5rem; right: 0;">

![](https://www.devmedia.com.br/arquivos/Artigos/23408/diagrama-caso-uso.png)

</span>

---

## Precificação

<span style="font-size: 1rem; width: 50%; display: inline-block; margin-top: 0; float: left; font-size: .86rem;">

🧮 Modelo de Estimativa Simplificada ( Baseado no método Pontos de Função )
| Complexidade | Critérios                                                                                                                                   | Pontos sugeridos |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- |
| **Simples**  | - Tela com poucos campos (até 5)<br>- Sem lógica de negócios<br>- CRUD básico (listar, cadastrar)                                           | 3 pontos         |
| **Médio**    | - Tela com 6 a 10 campos<br>- Tem lógica ou validações<br>- Relaciona com 1 ou 2 entidades<br>- Uploads ou filtros simples                  | 5 pontos         |
| **Complexo** | - Tela com mais de 10 campos<br>- Lógica de negócio significativa<br>- Personalizações dinâmicas<br>- Relatórios, assinaturas, modo offline | 8 pontos         |

🛠️ Fatores de Ajuste

| Fator                      | Impacto (%) | Quando aplicar                         |
| -------------------------- | ----------- | -------------------------------------- |
| Integração com API externa | +10 a 20%   | Se for integrar com sistemas terceiros |
| Suporte offline            | +15%        | Para PWA, IndexedDB, etc.              |
| Responsividade extra       | +10%        | Se envolver tablets, celulares e PC    |
| Segurança avançada         | +10%        | Ex: Criptografia, controle de acesso   |
</span>

<span style="position: absolute; width: 40%; top: 5rem; right: 0; font-size: 0.85rem;">

🧠 Dicas práticas:
    
Se estiver em dúvida, pense:

Tem lógica ou apenas exibe dados?

    Lógica? → Médio ou Complexo

Tem personalização ou é padrão?

    Personalizado? → Complexo

Precisa integrar com outras funções (ex: assinatura, upload)?

    Integra? → Complexo

Para sistemas simples: use 1h por ponto.

Para sistemas com muita lógica ou integração: use até 2h por ponto.

Valor por ponto = (Valor da hora) × (Horas estimadas por ponto)

[Planilha de Preços](https://docs.google.com/spreadsheets/d/19E__F9qoIvOXFIrDGJTBpDjYWBebUtsj/edit?usp=sharing&ouid=114030697287765904573&rtpof=true&sd=true)

</span>