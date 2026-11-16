<div align="center">

<img src="src/main/resources/logo.png" alt="Logo de Arthou’s Inventory View" width="120">

<h1>Arthou’s Inventory View</h1>
<p>Abra inventários e ender chests de jogadores com menus administrativos.</p>
<p><strong>Minecraft 1.21.1 · NeoForge · Java 21</strong></p>

</div>

[Instalação](#instalação) · [Uso](#uso) · [Como funciona](#como-funciona) · [Créditos](#créditos)

## Instalação

Coloque o JAR `build/libs/arthous-invview-neoforge-1211-1.0.0.jar` na pasta `mods/` do servidor. Quem joga pode entrar com o cliente padrão.

| Minecraft | Loader | Java | Versão do mod |
| --- | --- | --- | --- |
| 1.21.1 | NeoForge 21.1.228 | 21 | 1.0.0 |

## Uso

Entre no servidor como operador com **permissão nível 2** e execute um dos comandos abaixo no chat. Os menus são abertos para quem executou o comando.

| Comando | O que abre |
| --- | --- |
| `/view inv <jogador>` | Inventário principal, armadura e mão secundária. |
| `/view echest <jogador>` | Ender chest do jogador. |
| `/view curios <jogador>` | Espaços da integração opcional com **Curios**. |
| `/view cosmetic <jogador>` | Espaços da integração opcional com **Cosmetic Armor Reworked**. |

## Como funciona

- As telas usam menus do Minecraft. Os comandos de inventário e ender chest aceitam também `/view inv modify <jogador>` e `/view echest modify <jogador>`. **Os atalhos sem `modify` também abrem edição nesta variante.**
- As alterações em jogadores conectados usam o inventário do servidor. Para jogadores offline conhecidos pelo servidor, o mod abre os dados salvos do jogador.
- Os menus extras ficam disponíveis quando o mod de equipamento correspondente fornece os espaços.
- Use o nome ou o perfil reconhecido pelo servidor. Se os dados do jogador não estiverem disponíveis, o comando informa o problema no chat.

## Créditos

Desenvolvimento e port por [Arthou](https://github.com/arthoou). As integrações usam as APIs de **Curios** e **Cosmetic Armor Reworked** quando presentes.

## Compilar

```bash
java -classpath gradle/wrapper/gradle-wrapper.jar org.gradle.wrapper.GradleWrapperMain build
```

A saída de distribuição aparece no caminho indicado em **Instalação**.
