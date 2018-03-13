A SQL Server datatools projects with an associated Jenkinsfile written using the opinionated declarative syntax that implements a build pipeline that:

- Checks the project out from SCM
- Uses msbuild to build the project into a DacPac file
- Spins up a container to deploy the DacPac to, the container spun up will use a unique name, the name of the branch suffixed by SQLLinux and a unqiue external port
- Deploys the DacPac to the container
- Tears down the container
