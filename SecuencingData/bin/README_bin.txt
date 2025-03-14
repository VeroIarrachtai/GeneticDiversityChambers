**bin** : It has scripts to obtain ordered metadata from the sequenced samples

```
| +--bin/     # Directory
|   +--Get-Size-Files.Rmd     # Script para conseguir tamaño de archivos y codigo md5
|   +--Infraspecific_Variation_Samples.Rmd     # Script para generar data frame con datos de muestras secuenciadas y metadatos
```


#Buscarlos en mi MAC M1 y agregarlos al repo los archivos size y md5

# Outputs del script Get-Size-Files.Rmd  
write.csv(tamaños, "../outputs/size_fasta_GBS.csv", row.names = FALSE)
ggsave("../outputs/size_fasta_GBS.png", width = 6, height = 4)
write.csv(tamaños, "../outputs/size_fasta_Epi-GBS.csv", row.names = FALSE)
write.csv(resultado, "../outputs/md5_fasta_GBS.csv", row.names = FALSE)
write.csv(resultado, "../outputs/md5_fasta_Epi-GBS.csv", row.names = FALSE)


# Outputs del script Infraspecific_Variation_Samples.Rmd  
write.csv(df_combined_GBS, "../outputs/df_GBS_metadata.csv", row.names = FALSE)
write.csv(df_combined_Epi_GBS, "../outputs/df_Epi_GBS_metadata.csv", row.names = FALSE)

