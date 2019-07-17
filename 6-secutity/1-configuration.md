#Configuration

Make sure that you keep up to date with the releases and use de improviments they bring.

##Errors and Warings 

Hide warning and errors while in production. Make that in your `php.ini` file or using `error_reporting()` function. Both take a numeric argument, susually in form of an expression built from the predefined errors constants.

Default and Recomended production settings:

	* display_erros = Off
	* log_errors  = On
	* error_reporting = E_ALL & ~E_DEPRECATED & ~E_STRICT 

These are also the settings that you can assume to be set in the Zend exame, unless the question states otherwise.

How the Flags Work Pagina 150, ler novamente

##Disabling Functions and Classes

You can disable a function using the directive `disable_functions` and disable classes using  `disable_classes`, in your `php.ini`. These settings cannot be changed at runtime and using others `.ini` files.

The functions `exec`, `passthru`, `shell_exec` and `system` are commonly disabled in `php.ini` file. The `DirectoryInterator` and `Directory` are classes that are commonly disabled too, because are commonly used by an attacker.


##PHP as an Apache Module

##PHP as a CGI Binary

