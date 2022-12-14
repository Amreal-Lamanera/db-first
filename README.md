# Dobbiamo definire la struttura di una tabella per memorizzare i dati delle auto usate messe in vendita da un concessionario.

##### Nome Tabella: catalogo auto usate

- id                    -> BIGINT           -> PRIMARY_KEY: UNIQUE, NOT_NULL, AUTO_INCREMENT;
- vin                   -> VARCHAR(17)      -> UNIQUE, NOT_NULL;
- targa                 -> VARCHAR(7)       -> UNIQUE, NOT_NULL;
- marca                 -> VARCHAR(255)     -> NOT_NULL;
- modello               -> VARCHAR(255)     -> NOT_NULL;
- data_produzione       -> DATE             -> NOT_NULL;
- km                    -> MEDIUM_INT       -> NOT_NULL;
- colore_carrozzeria    -> VARCHAR(20)      -> NULLABLE;
- colore_interni        -> VARCHAR(20)      -> NULLABLE;
- num_possessori        -> TINYINT          -> DEFAULT(1);
- data_arrivo           -> DATE             -> NULLABLE;
- prezzo                -> FLOAT(8,2)       -> NOT_NULL;

##### Nome Tabella: equipaggiamento di serie vettura
- vin                   -> VARCHAR(17)      -> PRIMARY_KEY: UNIQUE, NOT_NULL
- cerchi_e_pneumatici   -> TEXT             -> NOT_NULL;
- comfort               -> TEXT             -> NULLABLE;
- elementi_di_comando   -> TEXT             -> NOT_NULL;
- esterni               -> TEXT             -> NOT_NULL;
- cerchi_e_pneumatici   -> TEXT             -> NOT_NULL;
- gruppi_ottici         -> TEXT             -> NOT_NULL;
- garanzia              -> TEXT             -> NULLABLE;
- infotainment          -> TEXT             -> NULLABLE;
- interni               -> TEXT             -> NOT_NULL;
- pacchetti_luce        -> TEXT             -> NULLABLE;
- sedili                -> TEXT             -> NOT_NULL;
- sicurezza             -> TEXT             -> NOT_NULL;
- sistemi_di_assistenza -> TEXT             -> NULLABLE;

##### Nome Tabella: equipaggiamento optional vettura
- vin                   -> VARCHAR(17)      -> PRIMARY_KEY: UNIQUE, NOT_NULL
- cerchi_e_pneumatici   -> TEXT             -> NULLABLE;
- comfort               -> TEXT             -> NULLABLE;
- elementi_di_comando   -> TEXT             -> NULLABLE;
- esterni               -> TEXT             -> NULLABLE;
- cerchi_e_pneumatici   -> TEXT             -> NULLABLE;
- gruppi_ottici         -> TEXT             -> NULLABLE;
- garanzia              -> TEXT             -> NULLABLE;
- infotainment          -> TEXT             -> NULLABLE;
- interni               -> TEXT             -> NULLABLE;
- pacchetti_luce        -> TEXT             -> NULLABLE;
- sedili                -> TEXT             -> NULLABLE;
- sicurezza             -> TEXT             -> NULLABLE;
- sistemi_di_assistenza -> TEXT             -> NULLABLE;