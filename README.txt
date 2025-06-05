# Terraform Azure Infrastrukturprosjekt

Dette prosjektet setter opp en webapplikasjon med en lastbalansert database-backend i Azure, organisert med Terraform-moduler.

## Innhold

Prosjektet består av:

- Virtuelt nettverk med subnet for web og database
- Én webserver (NGINX + MySQL-klient)
- To databasenoder (MySQL)
- Azure Load Balancer for database-trafikk
- Nettverkssegmentering og NSG-regler


## 🚀 Kom i gang

### Forutsetninger

- Terraform installert
- Azure CLI installert og logget inn

# For å lage SSH-nøkkel kan du benytte denne kommandoen
ssh-keygen -t rsa -b 4096 -f C:\ssh\azure_id_rsa

Kopier innholdet og legg til terraform.tvars
Legg til ssh_public_key = " din rsa ssh-key "

### Kjør Terraform

```bash
terraform init
terraform plan
terraform apply
```

## 🧹 Opprydding

```bash
terraform destroy
```

