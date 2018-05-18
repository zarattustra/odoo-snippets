###### Hacer sólo lectura un formulario cuando se cumplen los criterios


```xml
<?xml version="1.0" encoding="UTF-8"?>
<odoo>
   <data>
   
      <record model="ir.ui.view" id="modulo.modelo_form">
         <field name="name">Modelo</field>
         <field name="model">modulo.modelo</field>
         <field name="context">{'form_no_edit':[('state','=','borrador')]}</field>
         <field name="arch" type="xml">

            <form >
            ...
            </form>
            
         </field>
      </record>
      
   </data>
</odoo>
```
