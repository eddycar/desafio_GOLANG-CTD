# __Sistema de reserva de turnos__

Se desea implementar una API que permita administrar la reserva de turnos para una clínica
odontológica. Esta debe cumplir con los siguientes requerimientos:

- __Administración de datos de odontólogos:__ listar, agregar, modificar y eliminar odontólogos. Registrar __apellido__, __nombre__ y __matrícula__ de los mismos. Se desea el desarrollo de un __CRUD__ para la entidad __Dentista__.
    - **POST:** agregar dentista.
    - **GET:** traer dentista por ID.
    - **PUT:** actualizar dentista.
    - **PATCH:** actualizar un dentista por alguno de sus campos.
    - **DELETE:**  eliminar dentista.

- __Administración de datos de los pacientes:__ listar, agregar, modificar y eliminar pacientes. De cada uno se almacenan: __nombre, apellido domicilio, DNI y fecha de alta.__ Se desea el desarrollo de un __CRUD__ para la entidad __Paciente__.

    - **POST:** agregar paciente.
    - **GET:** traer paciente por ID.
    - **PUT:** actualizar paciente.
    - **PATCH:** actualizar un paciente por alguno de sus campos.
    - **DELETE:**  eliminar paciente.


- __Registrar turno:__ se tiene que poder permitir asignar a un __paciente__ un turno con un __odontólogo__ a una determinada __fecha y hora.__ Al turno se le debe poder agregar una __descripción__. Se desea el desarrollo de un __CRUD__ para la entidad __Turno__.

    - **POST**: agregar turno.
    - **GET**: traer turno por ID.
    - **PUT**: actualizar turno.
    - **PATCH**: actualizar un turno por alguno de sus campos.
    - **DELETE**: eliminar turno.
    - **POST**: agregar turno por DNI del paciente y matrícula del dentista.
    - **GET**: traer turno por DNI del paciente. Debe traer el detalle del turno (Fecha-Hora, descripción, Paciente y Dentista).

## __Requerimientos técnicos__

La aplicación debe ser desarrollada en diseño orientado a paquetes:

- **Capa/dominio de entidades de negocio.**
- **Capa/dominio de acceso a datos (Repository).**
- **Capa de acceso a datos (base de datos):** es la base de datos de nuestro sistema.
Podrás utilizar cualquier base de datos relacional modelado a través de un modelo entidad-relación, como H2 o MySQL, o no relacional, como MongoDB.

- **Capa/dominio service.**
- **Capa/dominio handler.**   