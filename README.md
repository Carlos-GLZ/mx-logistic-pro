# mx-logistic-pro - Infra + App (AWS CLI)

## Resumen
Infraestructura mínima en Free Tier: VPC, Subnet pública, IGW, Route Table, Security Group (22/80), EC2 (Amazon Linux), Elastic IP y buckets S3 para rutas, evidencias y logs.

## Pasos rápidos
```bash
cd infra
cp variables.example.env variables.env
# edita variables.env
chmod +x create_infra.sh destroy_infra.sh
./create_infra.sh
# al final obtendrás infraestructura-info.txt con IP, IDs, buckets, etc.