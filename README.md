Se describe enseguida el procedimiento a seguir para realizar una carga incremental de datos utilizando una herramienta de orquestación de datos de Azure, 
desde una base de datos en Sql-Server. El objetivo es comprender a detalle los pasos que el pipeline realiza, en cada una de sus actividades, inputs de entrada y salidas, 
así como realizar dos corridas del pipeline: 1 considerando los datos iniciales y una segunda al añadir datos a la fuente original. El pipeline a desarrollar, el cual consiste 
de dos actividades Lookup para obtener la última y la nueva fecha de actualización, para la carga del delta de datos(datos nuevos no incluidos en la tabla objetivo o target) y 
un stored procedure para actualizar el nuevo valor de la última fecha de actualización.
