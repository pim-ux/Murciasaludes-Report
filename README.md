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



| Problem + Description | Success Criteria | Priority | Soluction | Observation |
| :---         | :---           | :---          | :---         | :---         | 
| Atributo lang definido como en-GB enquanto o conteúdo está em espanhol | [2.4.1: Bypass Blocks (A)](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks) | Moderada | Alterar para lang="es-ES" para refletir o idioma do conteúdo. | ![Descrição](./Capturadeecrã2024-11-05,às23.32.51.png) |
| **Uso inadequado de aria-level** usar aria-level é redundante quando se usa um cabeçalho HTML que já tem um nível de hierarquia definido.| [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta | Remover aria-level e usar apenas cabeçalhos | Teste  |
| href Apontando para Arquivo de Imagem    | [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html) | Alta  | Remover o link da imagem e criar um card com um link esticado | Observation  |
| git diff     | The HTML heading element has an explicit aria-level="..." attribute.       | [1.3.1: Info and relationships (A)](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html)      |

## Report Contacto
Page: https://www.murciasalud.es/en/web/cuidar-y-paliar/contacto
