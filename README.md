# Internship
#include <stdio.h>

int main(void){

	float calculate_electricity_rates;
    int voltage;
    float current;
    float current_rate;
    
    // Calculate power in watts
    float power = voltage * current;
    
    // Calculate energy consumed in kWh
    float energy = (power * 1 * 1000) / (1000 * 60 * 60);
    
    // Calculate the hourly rate
    float hourly_rate = energy * (current_rate / 100);
    
    // Calculate the daily rate
    float daily_rate = hourly_rate * 24;
    
    printf("Hourly rate: %f\n", hourly_rate);
    printf("Daily rate: %f\n", daily_rate);
    
    return 0;
}
