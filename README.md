# helm
=> helm is a package manager for kubernetes.
=> helm uses a packaging format called "charts"
=> helm command line tool  allows us to interact with helm charts
=> set up HELM
  " curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
    chmod 700 get_helm.sh
    ./get_helm.sh "
=> helm list -a
=> will create own helm " helm create webapp" ( it creates folder in that we have all the structure )
=> " ls webapp "
=> remove all the files in template " rm -r webapp/template "
=> create our own yaml files in webapp/template --> deployment.yaml, service.yaml
=> create own values.yaml file in webapp
=> before applying changes will  do  dry run to check the values
    " helm install <chart-name> <helm-name> --dry-run --debug
    " helm install login webapp --dry-run --debug
=> " helm install login webapp" will do the deployment.
