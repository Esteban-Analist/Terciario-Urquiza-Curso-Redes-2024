```mermaid
classDiagram
    class Dinosaurio {
        +String Poder
        +String Velocidad
        +String Cosa copada
    }

    class Rataplasma {
        +String texto
        +String gato
        +String Siesta
    }

    class Paleontologo {
        +String Jorge gorno
        +String Jorge Paquez
    }

    class SinIdeas {
        +String name
        +List<Book> books
        +List<Member> members
        +List<Librarian> librarians
        +addMember(Member member)
        +removeMember(Member member)
    }

    Libro --> Dinosaurio : contiene
    Miembro --> Rataplasma : registra
    bibliotecario --> SinIdeas : administra
    Paleontologo --> Dinosaurio : investiga
    Paleontologo --> Rataplasma : Come
