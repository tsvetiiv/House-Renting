pipeline{
    agent{
        label "node"
    }
    stages{
        stage("Restore the project"){
            bat "dotnet restore"
        }
        stage("Build the project"){
            bat "dotnet build --no-restore"
        }
        stage("Run and tests"){
            bat "dotnet test --no-build --verbosity normal"
        }

    }
}