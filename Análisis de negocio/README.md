# Descripción del proyecto

Nos han ofrecido hacer prácticas en el departamento analítico de Y.Afisha. La primera tarea es ayudar a optimizar los gastos de marketing.

Lo que tienes:

- registros del servidor con datos sobre las visitas a Y.Afisha desde enero de 2017 hasta diciembre de 2018;
- un archivo con los pedidos en este periodo;
- estadísticas de gastos de marketing.

Lo que vas a investigar:

- cómo los clientes usan el servicio;
- cuándo empiezan a comprar;
- cuánto dinero aporta cada cliente a la compañía;
- cuándo los ingresos cubren el costo de adquisición de los clientes.


**Visitas:**

¿Cuántas personas lo usan cada día, semana y mes?
¿Cuántas sesiones hay por día? (Un/a usuario/a puede tener más de una sesión).
¿Cuál es la duración de cada sesión?
¿Con qué frecuencia los usuarios y las usuarias regresan?

**Ventas:**
 
¿Cuándo la gente empieza a comprar? (En el análisis de KPI, generalmente nos interesa saber el tiempo que transcurre entre el registro y la conversión, es decir, cuando el/la usuario/a se convierte en cliente. Por ejemplo, si el registro y la primera compra ocurren el mismo día, el/la usuario/a podría caer en la categoría Conversion 0d. Si la primera compra ocurre al día siguiente, será Conversion 1d.  Puedes usar cualquier enfoque que te permita comparar las conversiones de diferentes cohortes para que puedas determinar qué cohorte o canal de marketing es más efectivo).
¿Cuántos pedidos hacen durante un período de tiempo dado?
¿Cuál es el tamaño promedio de compra?
¿Cuánto dinero traen? (LTV)

**Marketing:**
 
¿Cuánto dinero se gastó? (Total/por fuente de adquisición/a lo largo del tiempo)
¿Cuál fue el costo de adquisición de clientes de cada una de las fuentes?
¿Cuán rentables eran las inversiones? (ROMI)


# Descripción de los datos

La tabla visits (registros del servidor con datos sobre las visitas al sitio web):

Uid: identificador único del usuario;
Device: dispositivo del usuario;
Start Ts: fecha y hora de inicio de la sesión;
End Ts: fecha y hora de término de la sesión;
Source Id: identificador de la fuente de anuncios de la que proviene el usuario.
Todas las fechas de esta tabla están en formato AAAA-MM-DD.

La tabla orders (datos sobre pedidos):

Uid: identificador único del usuario que realiza un pedido;
Buy Ts: fecha y hora del pedido;
Revenue: ingresos de Y.Afisha de este pedido.
La tabla costs (datos sobre gastos de marketing):

source_id: identificador de la fuente de anuncios
dt: fecha;
costs: gastos en esta fuente de anuncios en este día.