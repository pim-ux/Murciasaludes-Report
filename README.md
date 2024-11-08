# Murciasaludes-Report

**Report Creator:** [Patricia](https://pim-ux.github.io/Portfolio/)

**Date:** Tue Nov 05 2024

## Scope

**Website:**   [https://www.murciasalud.es/](https://www.murciasalud.es/)

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
[View page](https://www.murciasalud.es/)
<br>
<br>

| Problem + Description | Success Criteria WACG | Priority | Soluction | Observation |
| :---         | :---           | :---          | :---         | :---         | 
| **Cookies are not the first focusable element"** If you are browsing with a keyboard or screen reader, you must scroll through the entire page to accept or close cookies. | [3.2.1: On focus (Level A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | High | Add tabindex="0" o the cookie modal and set the focus automatically via JavaScript. Add semantics `div role="dialog" tabindex="0" aria-modal="true" aria-label="Manage Cookies">`| <img width="1196" alt="Modal de cookies" src="https://github.com/user-attachments/assets/5bb6ac13-c890-4459-8dba-c06998cd4611"> |
| **Missing ‘Skip to main content’ link**  | [2.4.1: Bypass Blocks (level A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | Hight | Add a link at the top of each page that allows you to jump directly to the main content `<a href="#conteudo-principal">Saltar para o conteúdo principal</a><main id="conteudo-principal"></main>`| |
| **`<main>` Inside an Element with Other Semantics** The `<main>` element helps to define the structure of the page and indicates that the main content begins. | [ 1.3.1: Informação e Relações (Level A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | High | Replace `<div class="main-content">` with the HTML5 element `<main>`. The `<main>` element must be unique per page and must not be nested within other semantic elements. | |
| **`lang` definido incorretamente** The content is in Spanish but the `lang` attribute is set to en-GB. | [2.4.1: Bypass Blocks (Level A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | Medium | Switch to `<html lang="es-ES>"` | |
| **Inadequate use of the aria-level** The use `aria-level` is redundant when using an HTML header that already has a defined hierarchy level.| [1.3.1: Info and relationships (level A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | High | Remove `aria-level` Use headings only. | ![Captura de ecrã 2024-11-06, às 16 22 50](https://github.com/user-attachments/assets/1b4abf05-1a0f-4c88-8d4e-2cf63221db34) |
| `href` points to an image file  | [1.3.1: Info and relationships (Level A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | High  | Remove the link (`<a href="...">`), leave only the `<img>` whith `alt=""` (`alt` empty) as it is a decorative image. | <img width="1086" alt="Captura de ecrã 2024-11-06, às 01 55 07" src="https://github.com/user-attachments/assets/952bbb55-090a-41c3-a451-7eab9e039e84"> |
| **Card com múltiplos links (um na imagem e outro no texto "leer más")** Navegação inconsistente: ao navegar por links, há 2 links diferentes que levam ao mesmo destino. | [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | High | O card deve ter apenas um único link que cubra toda a área clicável  [Exemplo construção](https://www.w3schools.com/bootstrap4/tryit.asp?filename=trybs_card_link&stacked=h)| <img width="1209" alt="Navegação por links com links duplicados" src="https://github.com/user-attachments/assets/a3049fff-9a98-4c05-b6f1-a13cf5cc528d"> |
| **Cabeçalhos escondidos, apenas disponíveis para leitores de ecrã.**  | [2.4.6: Cabeçalhos e Rótulos (Level AA)](https://www.w3.org/WAI/WCAG21/Understanding/headings-and-labels.html) | Moderada | A hierarquia e a organização do conteúdo deveriam ser compreensíveis tanto visualmente quanto para quem usa leitores de ecrã. | <img width="1143" alt="Leitor de ecrã titulos escondidos" src="https://github.com/user-attachments/assets/c5f91290-1608-4b68-850c-1e6916a4ed9c"> |
| **As hiperligações só se diferenciam do texto normal pela cor** Utilizadores com dificuldade de visão (daltonicos) podem não perceber a mudança de cor ou achar que os links não estão suficientemente destacados  | [1.4.1: Use of Color  (Level A)](https://www.w3.org/WAI/WCAG21/Understanding/use-of-color) | Alta () | Usar o sublinhado para links no meio do texto `<a href=".." class="anchor" > .agora-anchor-text-primary>...</a>` `text-decoration-line:underline; text-decoartion-style:solid; text-decoration-thickness:.094rem; text-decoration-color:#4772d8; text-underline-offset: .388rem;`| <img width="1302" alt="Captura de ecrã 2024-11-06, às 02 09 28" src="https://github.com/user-attachments/assets/dc2b0438-03d6-4995-a11f-433b9e056723">|

<br>
<br>

### Contacto
[View page](https://www.murciasalud.es/en/web/cuidar-y-paliar/contacto)
<br>
<br>

| Problem + Description | Success Criteria | Priority | Soluction | Observation |
| :---         | :---           | :---          | :---         | :---         | 
| **Falta required**  | [1.3.1: Info and Relationships  (Level A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | Adicionar required ao campo de input `<input class="ddm-field-text form-control" name="NombreYApellidos" type="text" required id="formInput_0">`| |
| **A associação entre o input e label deveria ser feita de forma semântica**  | [1.3.1: Info and Relationships  (Level A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | O uso de `aria-describedby` é útil para associar mensagens de erro ou informações extras ao campo, mas a associação entre o input e o label deve ser feita com o uso de for no `<label>` e id no `<input>`.||




