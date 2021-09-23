#include <iostream>

int main()
{
    
    //BMI Calculator - First Project

    float weightKG, heightM, bmiResult;

    std::cout << "Enter your current height in Meters: " << std::endl;
    std::cin >> heightM;
    
    std::cout << "Enter your current weight in KG: " << std::endl;
    std::cin >> weightKG;


    bmiResult = weightKG / (heightM * heightM);
    
    if(bmiResult < 18.5)
    {
        std::cout << "You are in the underweight range." << std::endl;
        std::cout << "Your BMI is: " << bmiResult << std::endl;
    }
    else if(bmiResult >= 18.5 && bmiResult <= 24.9)
    {
        std::cout << "You are in the normal weight range." << std::endl;
        std::cout << "Your BMI is: " << bmiResult << std::endl;
    }
    else if(bmiResult >= 25 && bmiResult <= 29.9)
    {
        std::cout << "You are in the overweight range." << std::endl;
        std::cout << "Your BMI is: " << bmiResult << std::endl;
    }
    else
    {
        std::cout << "You are in the obese range." << std::endl;
        std::cout << "Your BMI is: " << bmiResult << std::endl;
    }
    
    
    
    return 0;
}
