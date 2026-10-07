# aws-mini-platform-argocd


command to update kubeconfig for the cluster:
aws eks update-kubeconfig --name eks-aws-terraform-mini-dev --region eu-west-1 --kubeconfig ~/.kube/config-aws-mini-platform



## kubectl --kubeconfig ~/.kube/config-aws-mini-platform apply -f apps/app-of-apps.yaml to sync for the first time. After that, ArgoCD will automatically sync the apps defined in this app-of-apps.yaml file.
      

#kubectl --kubeconfig ~/.kube/config-aws-mini-platform apply -f apps/projects.yaml


k9s --kubeconfig ~/.kube/config-aws-mini-platform


aws resourcegroupstaggingapi get-resources \                                                                                
--tag-filters Key=Name,Values=aws-terraform-mini \
--query "ResourceTagMappingList[].ResourceARN" \
--output table