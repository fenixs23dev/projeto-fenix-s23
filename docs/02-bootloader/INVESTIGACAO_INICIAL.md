# FÊNIX-002 — Investigação Inicial do Bootloader

Data da coleta: 2026-11-14

## 1. Identificação do dispositivo

- Modelo: Samsung Galaxy S23
- Código do modelo: SM-S911B
- Codinome: dm1q
- SoC: Qualcomm SM8550
- Android: 17

## 2. Resultados originais

| Propriedade | Resultado |
|---|---|
| ro.bootloader | S911BXXUAGZIF |
| ro.boot.flash.locked | 1 |
| ro.boot.verifiedbootstate | green |
| ro.boot.vbmeta.device_state | locked |
| ro.boot.other.locked | 1 |
| ro.boot.veritymode | enforcing |
| ro.boot.slot_suffix | vazio |
| ro.build.ab_update | false |
| ro.build.version.release | 17 |
| ro.build.version.security_patch | 2026-10-05 |
| ro.product.model | SM-S911B |
| ro.oem_unlock_supported | vazio |
| sys.oem_unlock_allowed | vazio |

## 3. Interpretação técnica

### 3.1 Estado do bootloader

A propriedade ro.boot.flash.locked retornou 1.

A propriedade ro.boot.vbmeta.device_state retornou locked.

Esses resultados indicam que o dispositivo iniciou em estado
de bootloader bloqueado.

### 3.2 Verified Boot

A propriedade ro.boot.verifiedbootstate retornou green.

A propriedade ro.boot.veritymode retornou enforcing.

Os resultados indicam que a verificação de integridade
da inicialização está ativa.

### 3.3 Sistema de atualização

A propriedade ro.build.ab_update retornou false.

A propriedade ro.boot.slot_suffix não retornou valor.

Isso não permite concluir sozinho qual é toda a arquitetura
de partições do aparelho.

### 3.4 Desbloqueio OEM

As propriedades:

- ro.oem_unlock_supported
- sys.oem_unlock_allowed

retornaram valores vazios.

Isso significa apenas que essas propriedades não forneceram
informações nesta coleta.

Não é prova de que o desbloqueio seja impossível.

## 4. Informações pendentes

- Verificar a disponibilidade da opção OEM Unlock na interface
  oficial de configurações.
- Confirmar as condições oficiais de desbloqueio para o SM-S911B.
- Identificar a cadeia de inicialização Qualcomm/Samsung.
- Investigar a estrutura de partições.
- Identificar componentes relacionados a UEFI e firmware.

## 5. Segurança e limitações

Nesta etapa foram executados somente comandos de leitura.

Nenhuma partição foi modificada.
Nenhum firmware foi instalado.
Nenhuma alteração no bootloader foi realizada.

## 6. Conclusão preliminar

O Galaxy S23 SM-S911B está atualmente inicializando
com o bootloader bloqueado e a verificação de integridade ativa.

A possibilidade de inicialização de um sistema operacional
alternativo permanece em investigação.

Nenhuma compatibilidade com Windows ARM nativo foi comprovada.

## 7. Próxima etapa

Investigar a documentação técnica da cadeia de inicialização
do Qualcomm SM8550 e as particularidades da plataforma Samsung.
