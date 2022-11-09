# My Notes Using this Template Repo

- Read all `make` command definitions
- running `make infra-up` there's a line in the terraform `main.tf` file that tries to `cd` into your repo 
after cloning it in the ec2 instance, it won't infer the correct name if you changed the name so you need to 
change it in the setup script in `main.tf`
- if you had the above step fail, you may need to kill previous ssh that has bound port 8081 locally, can run: 
`kill -9 $(lsof -ti:8081)`

