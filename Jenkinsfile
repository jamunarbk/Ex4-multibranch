pipeline { 
agent any
stages { 
stage('Build') { 
steps { 
echo "Build step" 
} 
} 
stage('Test') { 
steps { 
script { 
if (isUnix()) { 
sh 'echo Testing code...' 
sh 'sleep 1' // simulate longer test if you want sh 'echo Tests completed' 
} else { 
bat 'echo Testing code...' 
bat 'echo Tests completed' 
} 
} 
} 
} 
stage('Deploy') { 
steps { 
echo "Deploy step" 
} 
} 
} 
}
