  int main() {
    stdio_init_all();
    printf("ADC Example, measuring GPIO26\n");
 
    adc_init(); 
    adc_gpio_init(27);
 
    adc_select_input(1);

   while (1) {

    const float conversion_factor = result * 3.3f / (1 << 12);
    uint16_t result = adc_read();
    printf("Raw value: 0x%03x, voltage: %2f temperatura: V\n", result, result * conversion_factor, result * conversion_factor /0.01); 
    sleep_ms(500);
   }
 }
