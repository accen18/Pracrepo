# Pracrepo

The CI Docker login jobs require `DOCKERHUBUSERNAME` and `DOCKERHUBPASSWORD`
GitHub Actions secrets. Configure both for each of the `Dev` and `Qa`
environments in the repository settings; the password should be a Docker Hub
access token for the corresponding username. In particular, the `Qa`
environment needs a non-empty `DOCKERHUBUSERNAME` for its login to succeed.
Pull requests from forks do not receive these secrets.