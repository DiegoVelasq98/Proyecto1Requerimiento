# Proyecto1Requerimiento
Proyecto1

LISTADO DE REQUERIMIENTOS
Requerimientos Funcionales (Globales y detallados)
El sistema permitirá:
- Administrar datos de Cliente (ABMC)&&&&&& Requerimiento Global
- Registrar Cliente &&&&&&&&&&&&&& Requerimiento detallado
- Modificar cliente
- Registrar baja de cliente
- Consultar clientes

• Administrar Servicios (ABMC de Servicios con tipo de prenda, tipo de servicio y precio)
- Registrar servicio de lavado
- Modificar servicio de lavado
- Registrar baja de servicio de lavado
- Consultar servicios

• Gestionar pedido de servicio de lavado de prendas (Transacción)
- Registrar pedido de servicio de lavado de prendas
- Cancelar pedido de servicio de lavado de prendas
- Consultar pedidos de servicio de lavado de prendas (Obs: Realizados por periodo y por estado)
- Controlar prendas no retiradas anulando pedidos (Será considerado como un control de pedidos los cuales se podrán anular luego de 90 días de no retirados)
- Gestionar lavado de prenda (Transacción ) (Obs: Este requerimiento global y el anterior pueden plantearse como uno solo)
- Consultar pedidos de servicio de lavado de prendas pendientes de realizar
- Registrar servicio de lavado de prendas realizado (Actualiza el estado de la prenda lista para entregar)
- Registrar imposibilidad de lavado de prendas

• Gestionar cobro de servicio (Transacción)
- Consultar pedidos de servicio de lavado de prendas listos para entrega al cliente
- Registrar cobro de servicio de lavado de prendas realizado y forma de pago
- Emitir comprobante de cobro (Ticket)
- Emitir cupón de tarjeta de crédito
- Anular cobro realizado
- Consultar cobros de servicios

• Administrar convenios con tarjetas de crédito/débito (ABMC de tarjetas de crédito/débito)
- Registrar convenio con tarjeta de crédito/débito
- Modificar convenio con tarjeta de crédito/débito
- Eliminar convenio con tarjeta de crédito/débito
- Consultar convenios con tarjeta de crédito/débito

• Generar reporte con los tipos de servicios de lavado de prendas solicitados (Generación deinforme)
- Emitir reporte de tipos de servicios de lavado de prendas mas solicitados 

# Documentar el diseño de la aplicación

# Propuesta

# Recepción

- Formulario para verificar si el cliente se encuentra registrado.
- Si el cliente no está registrado, entonces se solicitan los siguientes datos personales ingresándolos en un formulario:
    - Nombre.
    - Apellido.
    - Domicilio:
        - Calle.
        - Número.
        - Apartamento.
        - Piso.
    - Barrio.
    - Teléfono.
- Asigna número de cliente con un identificador único de la base de datos.

# Clasificación

- Menú de selección de tipo de servicio para cada una de las prendas que deja.
- Genera pedido llenando un formulario con los siguientes datos:
    - Número de pedido.
    - Fecha de pedido.
    - Tipos de prendas.
    - Tipos de servicio para cada prenda.
    - Cantidad de prendas por cada tipo de servicio.
    - Fecha pautada para devolución o entrega.
- El formulario realizado se imprime en duplicado, entregando el original al cliente.

# Lavado

- Menú de selección de para tipo de lavado.
- Tipo de servicio:
    - Lavado a seco.
    - Máquina lavadora.
- Tipo de prenda:
    - Blusa, lavado a seco: Q150.00
    - Blusa, máquina lavadora: Q110.00
    - Acolchado, lavado a seco: Q380.00
    - Acolchado, máquina lavadora: Q300.00

# Devolución de las prendas

- Valida que el pedido está listo para la devolución y lo coloca en estado “preparado”.
- Emisión e impresión de ticket por cobro del servicio prestado.
- El ticket se emite según reglamentación y regulación vigente de SAT para el registro del sistema de cobro.

# Cláusula de devolución

- El cliente cuenta con 90 días después de la fecha pactada para retirar las prendas, tiempo durante el cual la aplicación estará enviando alertas de reducción de tiempo para el retiro.

# Insumos para funcionamiento

- La aplicación cuenta con un módulo de inventario de insumos para garantizar el abastecimiento de los mismos para el funcionamiento de la lavandería.
- La aplicación contará con indicadores semanales de las existencias de insumos.
- La aplicación tendrá la facilidad para emitir un reporte mensual de los tipos de servicios de lavado más solicitados.

# Documentación de Análisis

# Propuesta

# Servicio de lavandería

- Una organización dedicada a ofrecer el servicio de lavado
- Establecer los servicios de lavado a brindar, precios
correspondientes y políticas de pago y entrega.
- Realizar la compra de productos e insumos para el lavado de las
prendas.

# Requisitos para Lavandería

- Investigar competencia
- Permiso de uso de suelos y certificación vigente
- Costo del local, Normas de sanidad y seguridad

# Reglas de negocio

- Pasados 90 días de la fecha de entrega pactada se pierde el derecho a retirar
las prendas.
- Pasado ese plazo la empresa puede disponer de las mismas.

# Identificación de Proceso

[]()

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/73ff64d2-8da3-4ab7-92bf-070cc46601ff/Untitled.png)

# Evaluaciones

- Ofrecer variedad y calidad de servicios ofreciendo descuentos por volumen de servicios diversos y que esto conlleve a la reducción de los precios
- Recepción: área donde la ropa es recibida en ampres o bolsas y aguarda a ser clasificada.
Área de clasificación: lugar donde los textiles son ordenados, por categoría textil y por grado de suciedad y color.
- Área de lavado: donde los textiles con lavados y equipada de lavadoras.
- Área de secado: área donde después de la extracción de agua Algunos tipos de tela pueden ser planchados directamente después del centrifugado, sin requerir secado.
- Área de almacenamiento: donde se almacena la ropa limpia hasta su distribución final.
- La lavandería deberá contar con áreas de soporte a funcionarios

# Recursos del proceso de lavado

- Encargado de Atención al Cliente
- Encargado de Lavado

# Servicios de lavado

## Objetivo

- Realizar el servicio de lavado de las prendas entregadas por el cliente con el cobro
respectivo.
- Cliente, persona quien requiere el servicio de lavado de prendas.
- Recomendar medidas para minimizar los riesgos de salud ocupacional en trabajadores de lavanderías.

# Clasificación de la ropa por precios

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cd2a6fd3-7744-4ccf-b63f-fedea2213980/Untitled.png)

La clasificación se debería realizar según el tipo de equipo en que van a ser secados o planchados o si van a ser totalmente secados o sólo acondicionados.

La lavandería deberá contar con áreas de soporte a funcionarios, como vestuarios, servicios sanitarios, etc. Área administrativa, de almacenamiento de equipos de aseo, y de almacenamiento de los productos químicos utilizados

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c564b1c2-115d-4a32-9f5d-cab769f31a21/Untitled.png)
