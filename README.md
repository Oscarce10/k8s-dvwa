# Kubernetes deployment



## Kubernetes cluster
### Create resources
```bash
kubectl create ns org-dvwa
kubectl apply -f . -n org-dvwa
```

### Retrieve web service and node port
```bash
kubectl get svc -n org-dvwa
```

### Retrieve pod status
```bash
kubectl get pods -n org-dvwa
```

## Next steps
- [ ] Go to the web service and configure DVWA: NodeIP:NodePort (Default:30001)
- [ ] Ensure security groups are properly configured to allow traffic to the NodePort
- [ ] Login to DVWA with default credentials: admin:admin
- [ ] Reset database
- [ ] Login to DVWA with default credentials: admin:password

## Troubleshooting
- Connection refused
  - Check VPN settings or try to disabling it temporarily and try again
