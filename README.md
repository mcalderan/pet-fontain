# pet-fontain

PIR pet drinker with arduino micro

Primo progetto con GitHub - Fontanella PIR per animali domestici con arduino micro

## Premesse

## Materiali
1. arduino nano
2. sensore livello liquido
3. rele SSD
4. pompa 12V
5. alimentatore 12V 2A
6. stepdown 12V-5V
7. modulo infrarossi PIR

## Funzionalità
La fontanella é costituita da un recipiente in materiale plastico di dimensioni adeguate.
Se il pin <!-- inserire il nr. pin--> del modulo infrarossi PIR è "1" (movimento nel campo di lavoro) viene controllato il livello sul pin #<!-- inserire il nr. pin-->. Se il pin # è "0" (livello OK) il pin # <!-- inserire il nr. pin--> diventa "1", inizia un timer sofware di # secondi e tramite il relè SSD la pompa 12V si accende, prelevando acqua dal fondo del recipiente tramite un tubo di pescaggio dotato di filtro da acquario e la reimmette nel recipiente.
Se il pin # è "1" (livello KO) la pompa non si attiva e si attiva il led sul pin <!-- inserire il nr. pin-->. Al termine del timer, il pin # <!-- inserire il nr. pin--> torna a "0"
