node {
    checkout scm
    def customImage = docker.build("python-hello_app:${env.BUILD_ID}")
	customImage.inside{
	 sh "./index.py"
	}
	//customImage.pull()
}
