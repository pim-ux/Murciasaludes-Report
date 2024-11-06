# Murciasaludes-Report

**Report Creator:** Patricia

**Date:** Tue Nov 05 2024

## Scope

**Website:** https://www.murciasalud.es/

**Scope of the website:** Portal oficial do Servicio Murciano de Salud

**WCAG Version:** 2.1

**Conformance target:** AAA

**Scenarios were tested using:**
- Keyboard-only interactions
- VoiceOver and NVDA with Google Chrome
- Colour Contrast Analyzer

## Summary

Reported on 1 of 55 WCAG 2.1 AAA
Success Criteria.
- 0 Passed
- 1 Failed


href Apontando para Arquivo de Imagem	1.3.1: Info and Relationships, 2.4.4: Link Purpose (In Context)	Moderada	Redirecionar href para uma página que exiba a imagem, ou usar target="_blank" para abrir em uma nova aba.


## Report Homepage
Page: https://www.murciasalud.es/

Falta de link "Saltar para o conteúdo principal"	2.4.1: Bypass Blocks	Alta	Adicionar um link visível e acessível no topo de cada página que permita saltar diretamente para o conteúdo principal.


| Problem + Description | Success Criteria | Priority | Soluction | Observation |
| :---         | :---           | :---          | :---         | :---         | 
| **Falta de link "Saltar para o conteúdo principal"**  | [2.4.1: Bypass Blocks (A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | Alta | Adicionar um link visível e acessível no topo de cada página que permita saltar diretamente para o conteúdo principal `<a href="#conteudo-principal">Saltar para o conteúdo principal</a><main id="conteudo-principal"></main>`| |
| **`<main>` Contido Dentro de um Elemento com Outra Semântica** O elemento `<main>` ajuda a definir a estrutura da página, sinalizando o início do conteúdo principal. | [ 1.3.1: Informação e Relações (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | Substituindo `<div class="main-content">` pelo elemento `<main>` do HTML5. O elemento `<main>` deve ser único por página e não deve estar aninhado dentro de outros elementos semânticos | |
| **`lang` definido incorretamente** Atributo lang definido como en-GB enquanto o conteúdo está em espanhol | [2.4.1: Bypass Blocks (A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | Moderada | Alterar para `<html lang="es-ES>"` para refletir o idioma do conteúdo. | ![Descrição](./Capturadeecrã2024-11-05,às23.32.51.png) |
| **Uso inadequado de aria-level** usar `aria-level` é redundante quando se usa um cabeçalho HTML que já tem um nível de hierarquia definido.| [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | Remover `aria-level` e usar apenas cabeçalhos | Teste  |
| `href` Apontando para Arquivo de Imagem    | [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta  | Remover o link da imagem e criar um card com um link esticado | Observation  |
| **Card com múltiplos links (um na imagem e outro no texto "leer más")** Navegação inconsistente: ao navegar por links, há 2 links diferentes que levam ao mesmo destino. | [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | O card deve ter apenas um único link que cubra toda a área clicável | <img width="1209" alt="Captura de ecrã 2024-11-05, às 23 33 27" src="https://github.com/user-attachments/assets/a3049fff-9a98-4c05-b6f1-a13cf5cc528d"> |
| **Cabeçalhos escondidos, apenas disponíveis para leitores de ecrã.**  | [2.4.6: Cabeçalhos e Rótulos (AA)](https://www.w3.org/WAI/WCAG21/Understanding/headings-and-labels.html) | Moderada | A hierarquia e a organização do conteúdo deveriam ser compreensíveis tanto visualmente quanto para quem usa leitores de ecrã. | <img width="1143" alt="Captura de ecrã 2024-11-05, às 23 32 51" src="https://github.com/user-attachments/assets/c5f91290-1608-4b68-850c-1e6916a4ed9c"> |





## Report Contacto
Page: https://www.murciasalud.es/en/web/cuidar-y-paliar/contacto
