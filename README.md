# datastax-studio-k8s

8 and 53

1. Download your astra secure connect bundle
2. Base64 encode the secure connect bundle

```
base64 secure-connect-bundle.zip
```

3. Open dsStudio.yaml
4. Copy the base64 output and paste it over changeme on line 8
5. Change line 53 to accept
6. kubectl create -f ./dsStudio.yaml
7. kubectl get services -n datastaxs
8. Navigate to the external ip given in step 7 (port 80) from your browser

When setting up a new connection in studio you can refrence the file above at bundles/filename.zip where the filename is defined at line 8

TODO: Update with better readme
