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

Success Criteria.
- 0 Passed
- 6 Failed

## List bug  

### Homepage
Link: https://www.murciasalud.es/
<br>
<br>

| Problem + Description | Success Criteria | Priority | Soluction | Observation |
| :---         | :---           | :---          | :---         | :---         | 
| **Falta de link "Saltar para o conteúdo principal"**  | [2.4.1: Bypass Blocks (A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | Alta | Adicionar um link visível e acessível no topo de cada página que permita saltar diretamente para o conteúdo principal `<a href="#conteudo-principal">Saltar para o conteúdo principal</a><main id="conteudo-principal"></main>`| |
| **`<main>` Contido Dentro de um Elemento com Outra Semântica** O elemento `<main>` ajuda a definir a estrutura da página, sinalizando o início do conteúdo principal. | [ 1.3.1: Informação e Relações (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | Substituindo `<div class="main-content">` pelo elemento `<main>` do HTML5. O elemento `<main>` deve ser único por página e não deve estar aninhado dentro de outros elementos semânticos | |
| **`lang` definido incorretamente** Atributo lang definido como en-GB enquanto o conteúdo está em espanhol | [2.4.1: Bypass Blocks (A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | Moderada | Alterar para `<html lang="es-ES>"` para refletir o idioma do conteúdo. | |
| **Uso inadequado de aria-level** usar `aria-level` é redundante quando se usa um cabeçalho HTML que já tem um nível de hierarquia definido.| [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | Remover `aria-level` e usar apenas cabeçalhos | |
| `href` Apontando para Arquivo de Imagem    | [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta  | Remover o link (`<a href="...">`), deixar apenas a `<img>` com `alt=""` (`alt` vazio) pois é uma imagem decorativa | <img width="1086" alt="Captura de ecrã 2024-11-06, às 01 55 07" src="https://github.com/user-attachments/assets/952bbb55-090a-41c3-a451-7eab9e039e84"> |
| **Card com múltiplos links (um na imagem e outro no texto "leer más")** Navegação inconsistente: ao navegar por links, há 2 links diferentes que levam ao mesmo destino. | [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | O card deve ter apenas um único link que cubra toda a área clicável  [Exemplo construção](https://www.w3schools.com/bootstrap4/tryit.asp?filename=trybs_card_link&stacked=h)| <img width="1209" alt="Captura de ecrã 2024-11-05, às 23 33 27" src="https://github.com/user-attachments/assets/a3049fff-9a98-4c05-b6f1-a13cf5cc528d"> |
| **Cabeçalhos escondidos, apenas disponíveis para leitores de ecrã.**  | [2.4.6: Cabeçalhos e Rótulos (AA)](https://www.w3.org/WAI/WCAG21/Understanding/headings-and-labels.html) | Moderada | A hierarquia e a organização do conteúdo deveriam ser compreensíveis tanto visualmente quanto para quem usa leitores de ecrã. | <img width="1143" alt="Captura de ecrã 2024-11-05, às 23 32 51" src="https://github.com/user-attachments/assets/c5f91290-1608-4b68-850c-1e6916a4ed9c"> |


<br>
<br>
<br>

### Contacto
Link: https://www.murciasalud.es/en/web/cuidar-y-paliar/contacto
<br>
<br>

| Problem + Description | Success Criteria | Priority | Soluction | Observation |
| :---         | :---           | :---          | :---         | :---         | 
| **Falta required**  | [1.4.1: Use of Color  (A)](https://www.w3.org/WAI/WCAG21/Understanding/use-of-color) | Alta |  | |

<br>
<br>
<br>

### Información sobre Historia Clínica Nacional y Europea
Link: https://www.murciasalud.es/en/informacion-sobre-hcdsns-ps
<br>
<br>

| Problem + Description | Success Criteria | Priority | Soluction | Observation |
| :---         | :---           | :---          | :---         | :---         | 
| **As hiperligações só se diferenciam do texto normal pela cor**  | [1.4.1: Use of Color  (A)](https://www.w3.org/WAI/WCAG21/Understanding/use-of-color) | Moderada | Usar o sublinhado para links no meio do texto| <img width="1302" alt="Captura de ecrã 2024-11-06, às 02 09 28" src="https://github.com/user-attachments/assets/dc2b0438-03d6-4995-a11f-433b9e056723">|

