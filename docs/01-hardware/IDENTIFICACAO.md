# FÊNIX-001 — Identificação do Hardware

Data do registro: 2026-11-14

## 1. Dispositivo de referência

- Fabricante: Samsung
- Modelo: SM-S911B
- Dispositivo/codinome: dm1q
- Plataforma: Qualcomm
- SoC identificado: SM8550
- Processador comercial: Snapdragon 8 Gen 2
- GPU: Adreno 740
- RAM declarada no README do projeto: 8 GB

## 2. Evidências coletadas no Termux

Comandos executados anteriormente:

    getprop ro.soc.model
    getprop ro.boot.hardware
    getprop ro.boot.verifiedbootstate
    getprop ro.product.device

Resultados registrados:

    SM8550
    qcom
    green
    dm1q

## 3. Interpretação

- SM8550 identifica a plataforma do SoC.
- qcom identifica a plataforma de hardware Qualcomm.
- dm1q identifica o dispositivo.
- green é o estado informado pelo Android Verified Boot.

O estado green não deve ser interpretado isoladamente como
prova de que o bootloader está bloqueado ou desbloqueado.

## 4. Informações ainda pendentes

- Estado de desbloqueio do bootloader.
- Versão completa do firmware.
- Versão do kernel Android.
- Mapa de partições.
- Cadeia de inicialização.
- Disponibilidade de documentação técnica específica.
- Compatibilidade de UEFI/EDK2.

## 5. Objetivo da próxima investigação

Identificar a cadeia de inicialização do SM8550 e as limitações
de segurança e firmware do SM-S911B.

## 6. Estado deste registro

Identificação inicial documentada.
Investigação técnica em andamento.
