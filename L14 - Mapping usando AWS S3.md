# Mapping usando AWS S3

**IICS** puede conectarse a servicios de **Amazon Web Services (AWS)** como **S3** o **Redshift**.

En este ejercicio crearemos un mapping para conectarnos a un **Bucket** de **AWS S3**

> Revisar la conexión **_conn_AWS_S3**.

Para entender su funcionamiento ejecutaremos los siguientes pasos:

1. Ingresamos a [IICS](https://dm-us.informaticacloud.com) y seleccionamos **Data Integration**.

![AWS](images/img_ism_01.png)

2. Del panel izquierdo seleccionamos **Explorar**, seleccionamos el proyecto **_pro_cap_iics** e ingresamos a nuestra carpeta. Estando es esta ruta, damos clic en el botón **Nuevo** que se encuentra en el panel izquierdo.

![AWS](images/img_ism_02.png)

3. Seleccionar **Mappings**->**Mapping**

![AWS](images/img_ism_06.png)

4. Establecer el nombre del mapping como **M_AWS_S3_trace_events**.

![AWS](images/img_aws_01.png)

5. Configurar **Source**->**Source** como se muestra en la siguiente imagen:

![AWS](images/img_aws_02.png)

6. Enlazar **Source** a **Target**.

7. Configurar **Target**->**Target** como se muestra en la siguiente imagen:

![AWS](images/img_aws_03.png)

> En la opción **Object** debemos dar clic en el botón **Select** para configurar el archivo de destino. En el nombre del archivo colocar como sufijo sus **iniciales** para identificarlo.

8. **Guardar**, **Validar** y Ejecutar (**Run**).

9. Seleccionar el agente seguro **vm-training** y dar clic en el botón **Run**.

10. Ir a **My Jobs** para monitorear la ejecución.

![AWS](images/img_aws_04.png)

11. Revisar los registros leídos y cargados.

![AWS](images/img_aws_05.png)
