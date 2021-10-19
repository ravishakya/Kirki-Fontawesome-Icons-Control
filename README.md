# Kirki Fontawesome Icons Control

**Author:** Ravi Shakya  
**Author URI:** https://bizbergthemes.com  
**License:** GNU General Public License v2 or later  
**License URI:** http://www.gnu.org/licenses/gpl-2.0.html  
**Version:** 0.1

## Description ##

Use this control to add fontawesome control in your customizer settings. By default it uses fontawesome 6 icons.

![image](https://user-images.githubusercontent.com/11089018/137852550-9ea887a5-5c74-406e-bc4f-d4f2d8710967.png)

## Example ##

````
Kirki::add_field( 'bizberg', array(
    'type'              => 'font-awesome-6',
    'label'             => 'Icon',
    'section'           => 'detail_page',
    'settings'          => 'icon',
    'priority'          => 1,
    'choices'           => array(
        'height'       => '200px',
        'search_icons' => true
    ),
    'default'           => json_encode(
        array(
            'icon'         => 'fas fa-ad',				
        )
    ) 
) );
````
In the above control you can control the height and search icons

**Parameters**  
````
Kirki::add_field( 'bizberg', array(
    -----------------------------
    'choices' => array(
        'height'       => '200px',
        'search_icons' => true
    ),
    -----------------------------
) );
````
**height**       - (string) (optional) Eg: '100px' , '200px'. **Default: '300px'**

**search_icons** - (boolean) (optional) If true, it will show a text box to search for icons. **Default : false**

````
Kirki::add_field( 'bizberg', array(
    -----------------------------
    'default' => json_encode(
        array(
            'icon' => 'fas fa-ad',		
        )
    ) 
    -----------------------------
) );
````
