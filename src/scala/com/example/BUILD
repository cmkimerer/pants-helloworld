scala_library(name='hello-world-scala-lib',
  dependencies=[],
  sources=globs('*.scala'),
  provides=artifact(org='com.example.scala',
                    name='hello-world-scala-lib',
                    repo='build-support/ivy-repo:public'
                    )
)

jvm_binary(name ='hello-world-scala-run',
  main='com.example.scala.HelloWorld',
  dependencies = [
    ':hello-world-scala-lib',
  ]
)
