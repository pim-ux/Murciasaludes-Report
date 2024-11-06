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

| Problem + Description | Success Criteria WACG | Priority | Soluction | Observation |
| :---         | :---           | :---          | :---         | :---         | 
| **Os cookies não é o primeiro elemento focável"** Ao navegar com teclado ou leitor de ecrã é preciso percorrer toda a página para Aceitar ou fechar os cookies | [3.2.1: On focus (A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | Alta | Adicionar tabindex="0" ao modal de cookies e configurar o foco automaticamente via JavaScript. Adicionar Semântica `div role="dialog" tabindex="0" aria-modal="true" aria-label="Manage Cookies">`| <img width="1196" alt="Modal de cookies" src="https://github.com/user-attachments/assets/5bb6ac13-c890-4459-8dba-c06998cd4611"> |
| **Falta de link "Saltar para o conteúdo principal"**  | [2.4.1: Bypass Blocks (A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | Alta | Adicionar um link visível e acessível no topo de cada página que permita saltar diretamente para o conteúdo principal `<a href="#conteudo-principal">Saltar para o conteúdo principal</a><main id="conteudo-principal"></main>`| |
| **`<main>` Dentro de um Elemento com Outra Semântica** O elemento `<main>` ajuda a definir a estrutura da página, sinalizando o início do conteúdo principal. | [ 1.3.1: Informação e Relações (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | Substituindo `<div class="main-content">` pelo elemento `<main>` do HTML5. O elemento `<main>` deve ser único por página e não deve estar aninhado dentro de outros elementos semânticos | |
| **`lang` definido incorretamente** Atributo lang definido como en-GB enquanto o conteúdo está em espanhol | [2.4.1: Bypass Blocks (A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | Moderada | Alterar para `<html lang="es-ES>"` para refletir o idioma do conteúdo. | |
| **Uso inadequado de aria-level** usar `aria-level` é redundante quando se usa um cabeçalho HTML que já tem um nível de hierarquia definido.| [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | Remover `aria-level` e usar apenas cabeçalhos | |
| `href` Apontando para Arquivo de Imagem    | [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta  | Remover o link (`<a href="...">`), deixar apenas a `<img>` com `alt=""` (`alt` vazio) pois é uma imagem decorativa | <img width="1086" alt="Captura de ecrã 2024-11-06, às 01 55 07" src="https://github.com/user-attachments/assets/952bbb55-090a-41c3-a451-7eab9e039e84"> |
| **Card com múltiplos links (um na imagem e outro no texto "leer más")** Navegação inconsistente: ao navegar por links, há 2 links diferentes que levam ao mesmo destino. | [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | O card deve ter apenas um único link que cubra toda a área clicável  [Exemplo construção](https://www.w3schools.com/bootstrap4/tryit.asp?filename=trybs_card_link&stacked=h)| <img width="1209" alt="Navegação por links com links duplicados" src="https://github.com/user-attachments/assets/a3049fff-9a98-4c05-b6f1-a13cf5cc528d"> |
| **Cabeçalhos escondidos, apenas disponíveis para leitores de ecrã.**  | [2.4.6: Cabeçalhos e Rótulos (AA)](https://www.w3.org/WAI/WCAG21/Understanding/headings-and-labels.html) | Moderada | A hierarquia e a organização do conteúdo deveriam ser compreensíveis tanto visualmente quanto para quem usa leitores de ecrã. | <img width="1143" alt="Leitor de ecrã titulos escondidos" src="https://github.com/user-attachments/assets/c5f91290-1608-4b68-850c-1e6916a4ed9c"> |
| **As hiperligações só se diferenciam do texto normal pela cor** Utilizadores com dificuldade de visão (daltonicos) podem não perceber a mudança de cor ou achar que os links não estão suficientemente destacados  | [1.4.1: Use of Color  (A)](https://www.w3.org/WAI/WCAG21/Understanding/use-of-color) | Alta () | Usar o sublinhado para links no meio do texto `<a href=".." class="anchor" > .agora-anchor-text-primary>...</a>` `text-decoration-line:underline; text-decoartion-style:solid; text-decoration-thickness:.094rem; text-decoration-color:#4772d8; text-underline-offset: .388rem;`| <img width="1302" alt="Captura de ecrã 2024-11-06, às 02 09 28" src="https://github.com/user-attachments/assets/dc2b0438-03d6-4995-a11f-433b9e056723">|

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


