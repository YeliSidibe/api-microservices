# Get Subscription Id
az account show --query id
Yeli Sidibe c74b1006-4a93-4234-a0f5-d633c2cbb13f

# Create a new service principal
az ad sp create-for-rbac --name "yeliContainerApp" --role contributor --scopes /subscriptions/c74b1006-4a93-4234-a0f5-d633c2cbb13f/resourceGroups/rg-container-apps-service --sdk-auth