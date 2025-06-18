# cicd-config-disclosure.yaml
Nuclei template + step-by-step guide to detect exposed CI/CD configuration files like Jenkinsfile, .git, Dockerfile, .env, and others—even under Cloudflare protection.

go install -v github.com/projectdiscovery/nuclei/v3/cmd/nuclei@latest

nuclei -u https://<> -t cicd-config-disclosure.yaml -o findings.txt
