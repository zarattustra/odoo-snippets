###### Usar vista especifica para cada acción
```xml
<?xml version="1.0" encoding="UTF-8"?>
<odoo>
   <data>
   
      <record model="ir.actions.act_window" id="modulo.modelo_w1">
         <field name="name">Ejemplo vista 1</field>
         <field name="res_model">modulo.modelo</field>
         <field name="view_mode">tree,form</field>
         <field name="view_id" ref="modulo.vista_arbol1" />
      </record>
      
      <record model="ir.actions.act_window" id="modulo.modelo_w2">
         <field name="name">Ejemplo vista 2</field>
         <field name="res_model">modulo.modelo</field>
         <field name="view_mode">tree,form</field>
         <field name="view_id" ref="modulo.vista_arbol2" />
      </record>
      
      <menuitem name="Menu" id="modulo.menu_root" />
      <menuitem name="submenu1" parent="modulo.menu_root" id="modulo.submenu1" action="modulo.modelo_w1"/>
      <menuitem name="submenu2" parent="modulo.menu_root" id="modulo.submenu2" action="modulo.modelo_w2"/>
      
   </data>
</odoo>
```
