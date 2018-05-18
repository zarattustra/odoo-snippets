###### Cargar fecha actual

<code>
from datetime import datetime
...
  fecha = fields.Date('Fecha de solicitud',required=True,default=datetime.today())
</code>
