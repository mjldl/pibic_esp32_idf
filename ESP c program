/*===============================================*/
/* --- Bibliotecas --- */
#include <stdio.h>
#include "freertos/FreeRTOS.h"
#include "freertos/task.h"
#include "driver/gpio.h"
#include "sdkconfig.h"
/*===============================================*/
/* --- Protótipos de funções --- */

/*===============================================*/
/* --- Programa --- */
static unint8_t s_led_state = 0;

void app_main(void) 
{
	gpio_reset_pin(CONFIG_BLINK_GPIO);
	gpio_set_direction(CONFIG_BLINK_GPIO, GPIO_MODE_OUTPUT);
	while (1) 
	{	
		gpio_set_level(CONFIG_BLINK_GPIO, s_led_state);
		s_led_state = !s_led_state
		vTaskDelay(CONFIG_BLINK_PERIOD);
	}
} /* end app_main */
/*===============================================*/
/* --- Desenvolvimento das funções --- */

/*===============================================*/

