pipeline{
    agent any
    stages{
        stage("Mostrar informacion segun dia de la semana"){
            steps{
                script{
                    def dia = new Date().getDay()
                    def map = [1:"Lunes", 2:"Martes", 3:"Miércoles", 4:"Jueves", 5:"Viernes",]
                    if(dia == 1){
                        echo ""
                    }
                    if(dia == 2){
                        echo "El usuario que ha ejecutado el trabajo es ${env.USER}"
                    }
                    if(dia == 3){
                        echo "El temperatura actual que hace en Madrid es de 16 grados Celsius"
                    }
                    if(dia == 4){
                        git branch: "main", url: "https://github.com/javigutierrezb/Curso_Jenkins.git"
                    }
                    if(dia == 5){
                        echo ""
                    }
                }
            }
        }
    }
}
