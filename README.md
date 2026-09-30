# AfterCutting — downloads

Binários públicos do **AfterCutting**, pipeline local de pós-produção fotográfica para Mac com
Apple Silicon: triagem, correção de cor e entrega. As fotos não saem do Mac, os pixels não são
reescritos (só metadados XMP) e nada é apagado.

Este repositório guarda só os instaladores. O código do app não fica aqui.

## Baixar

[**AfterCutting para macOS (Apple Silicon)**](https://github.com/Sanzuka/aftercutting-releases/releases/latest/download/AfterCutting-arm64.dmg)
— sempre a versão mais recente. Versões anteriores em [Releases](https://github.com/Sanzuka/aftercutting-releases/releases).

## Requisitos

- Mac com Apple Silicon (M1, M2, M3 ou M4). Não roda em Mac com Intel.
- [exiftool](https://exiftool.org): `brew install exiftool`

## Instalação

1. Abra o `.dmg` e arraste o **AfterCutting** para **Aplicativos**.
2. Enquanto o app não é notarizado pela Apple, o macOS bloqueia a primeira abertura. Libere de
   uma destas formas:
   - **Ajustes do Sistema › Privacidade e Segurança** → *Abrir Mesmo Assim*, depois de tentar abrir uma vez; ou
   - no Terminal: `xattr -dr com.apple.quarantine /Applications/AfterCutting.app`
3. Abra o AfterCutting normalmente.

## Conferir o arquivo

Cada release traz o SHA-256 do `.dmg` nas notas. Para conferir:

```bash
shasum -a 256 ~/Downloads/AfterCutting-arm64.dmg
```
