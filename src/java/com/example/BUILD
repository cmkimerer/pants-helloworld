java_library(name='hello-world-java-lib',
  dependencies=[],
  sources=globs('*.java'),
  provides=artifact(org='com.example.java',
                    name='hello-world-java-lib',
                    repo='build-support/ivy-repo:public'
                    )
)

jvm_binary(name ='hello-world-java-run',
  main='com.example.java.HelloWorld',
  dependencies = [
    ':hello-world-java-lib',
  ]
)
