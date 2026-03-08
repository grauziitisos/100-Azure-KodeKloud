#Create a Virtual Network (VNet) named nautilus-vnet in the centralus region with any IPv4 CIDR block.
az network vnet create \
  --name nautilus-vnet \
  --resource-group `az group list --query "[0].name" -o tsv` \
  --location centralus \
  --address-prefix 10.0.0.0/16
