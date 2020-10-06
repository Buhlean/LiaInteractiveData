<!--
author: Alexander Buhl

script: https://cdn.jsdelivr.net/gh/Buhlean/LiaInteractiveData/src/Module.min.js

@data
<script>console.log('@0: ' + @1);</script>
@end

@calculations
<script>console.log('@0: ' + @1);</script>
@end

@subtotal
<script>console.log('@0: ' + @1);</script>
@end

@input
<script>console.log('@0: ' + @1);</script>
@1 @2
@end

@output
<script>console.log('@0: ' + @1);</script>
0 @2
@end

-->
[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/Buhlean/LiaInteractiveData/master/Module.md)

# Module Interactive Data

.

## Try it!

.

@data(gallons_consumed_per_day, 378000000)
@data(budget, 3000000000)
@data(rebate, 3500)
@data(overhead, 100000000)
@data(low_miles_per_gallon, 17)
@data(high_miles-per_gallon, 24)
@data(car_lifetime_miles, 150000)
@data(average_miles_left_percent, 25)
@data(kg_co2_per_gallon_gas, 8.87)
@data(co2_per_co2equivalent, 0.95)
@data(tons_co2equivalent_emitted_yearly, 6983000)
@data(dollars_per_gallon, 3)


@subtotal(cars_traded, (budget-overhead)/rebate)
@subtotal(old_mpgs, 1)

@subtotal(gallons_saved, gallons_saved_per_car
@subtotal(gallons_consumed_per_hour, gallons_consumed_per_day/24)
@subtotal(hours_of_gas, gallons_saved/gallons_consumed_per_hour

Say we allocate @input(budget, 3000000000, $, billions, de-de) for the following program: Car-owners who trade in an old car that gets less than @input(low_miles_per_gallon, 17, MPG,,), and purchase a new car that gets better than @input(high_miles_per_gallon, 24, MPG,,), will receive a @input(rebate, 3500, $,,de-de) rebate.

We estimate that this will get @output(cars, (budget-overhead)/rebate,,,de-de) old cars off the road. It will save @output(gallons_saved, 1068000000, gallons of gas, millions, de-de) (or @output(hours_consumption, gallons_saved/gallons_consumed_per_hour, hours, hours, de-de) worth of U.S. gas consumption.) It will avoid @output(tons_co2, 9970000, million tons CO2, millions,de-de), or @output(annual_greenhouse_gas, 0.14, %, percent, de-de) of annual U.S. greenhouse gas emissions.

The abatement cost is @output(dollars_per_ton, budget/tons_saved, $ per tons,,de-de) CO2e of federal spending, although it’s @output(dolars_per_ton_balanced, -20, $ per ton,,de-de) CO2e on balance if you account for the money saved by consumers buying less gas.

