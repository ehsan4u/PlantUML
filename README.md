# PlantUML

How to use

@startuml
class Object << general >>
Object <|--- ArrayList : parent

note top of Object : In java, every class\nextends this one.

note "This is a floating note" as N1
note "This note is connected\nto several objects." as N2
Object .. N2
N2 .. ArrayList : a message

class Foo {
  -privateField
  +publicField
  #protectedField
  ~classProtected
  styled method01();
  void method02();
}
note bottom: On last defined class

Foo -[hidden]> Object
@enduml