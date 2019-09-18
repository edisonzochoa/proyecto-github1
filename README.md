# proyecto-github1
En este proyecto se busca diseñar antenas de microcinta para la captacion y transferencia de energia por medio inalambrico.
Para obtener un algoritmo de optimizacion y mejorar las antenas se busca la integracion entre los sotfware matlab y cst-studio.



![alt text](https://user-images.githubusercontent.com/47603954/64968449-d0556800-d867-11e9-8654-f217807a39d0.jpg)
Repositorio de scripts de proyecto-github1

# Diagrama de bloques integracion matlab-cst
![alt text](https://user-images.githubusercontent.com/47603954/64974930-79ee2680-d873-11e9-94a8-f502ce1488d6.gif)

# Utilizando el software GNURadio para detectar frecuencia y anchos de banda.
! [alt tex](https://user-images.githubusercontent.com/47603954/64459834-8bd70900-d0be-11e9-94b4-5a9f4bd2a3fe.PNG)

#Introduccion a GNURadio desde python 
#! / Usr / bin / env Python 
####################################### ########### 
# Gnuradio Python Flow Graph 
# Título: Tutorial Three 
# Tomado de:https://wiki.gnuradio.org/index.php/Guided_Tutorial_GNU_Radio_in_Python
############# ###################################### 

desde  gnuradio  import  analog 
desde  gnuradio  import  audio 
desde  gnuradio  import  eng_notation 
de  gnuradio  import  gr 
de  gnuradio.eng_option  import eng_option 
de  gnuradio.filter  import  firdes 
de  optparse  import  OptionParser 

class  tutorial_three ( gr . top_block ): 

    def  __init__ ( self ): 
        gr . top_block . __init__ ( self ,  "Tutorial Three" ) 

        ####################################### ########### 
        # Variables 
        ################################################## 
        auto . samp_rate  =  samp_rate  =  32000 

        ############################################ ####### 
        # Bloques 
        ####################################### ########### 
        auto . audio_sink_0  =  audio . sink ( samp_rate ,  "" ,  True ) 
        self . analog_sig_source_x_1  =  analógico . sig_source_f ( samp_rate , analógico . GR_SIN_WAVE ,  350 ,  . 1 ,  0 ) 
        auto . analog_sig_source_x_0  =  analógico . sig_source_f ( samp_rate ,  analógica . GR_SIN_WAVE ,  440 ,  . 1 ,  0 ) 

        ################################# ################# 
        # Conexiones 
        ############################# ##################### 
        auto . conectar (( auto. analog_sig_source_x_1 ,  0 ),  ( self . audio_sink_0 ,  1 )) 
        self . connect (( self . analog_sig_source_x_0 ,  0 ),  ( self . audio_sink_0 ,  0 )) 


# QT sumidero reimplementación del método 

    def  get_samp_rate ( self ): 
        return  self . frecuencia de muestreo 

    def  set_samp_rate ( self ,  samp_rate ): 
        self . samp_rate  =  samp_rate 
        self . analog_sig_source_x_0 . set_sampling_freq ( self . samp_rate ) 
        self . analog_sig_source_x_1 . set_sampling_freq ( self . samp_rate ) 

if  __name__  ==  '__main__' : 
    parser  =  OptionParser (option_class = eng_option ,  use = "% prog: [opciones]" ) 
    ( opciones ,  argumentos )  =  analizador . parse_args () 
    tb  =  tutorial_three () 
    tb . start () 
    raw_input ( 'Presione Enter para salir:' ) 
    tb . parada () 
    tb . esperar ()





# Diagrama de bloques waterfall deteccion de ruido
! [alt tex](https://user-images.githubusercontent.com/47603954/64459940-cccf1d80-d0be-11e9-8eab-44f07b01e18e.PNG)



# Diagrama de flujo waterfall
! [alt tex](https://user-images.githubusercontent.com/47603954/64460001-ed977300-d0be-11e9-9c0d-2b75362b1595.PNG)


# Diagrama de bloques generador de señales
! [alt tex](https://user-images.githubusercontent.com/47603954/64459910-b923b700-d0be-11e9-98d2-4b90bfe9124f.PNG)


