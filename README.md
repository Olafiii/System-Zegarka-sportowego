# System-Zegarka-sportowego
System który zbiera i przetwarza dane z zegarka sportowego, do poszczególnych aktywności i przypisuje je do konkretnego użytkownika.
user - klasa z właściwościami userID, firstName, age, height, weight i metodą DisplayProfile()
smartWatch - klasa z właściwościami watchID, model, batteryLevel, owner(user) i metodami 
startActivity(), showBatteryStatus()
activity - klasa abstrakcyjna z właściwościami activityID, date, durationMinutes, distanceKm i metodami CalculateCalories(abstrakcyjna), showSummary()
Użytkownik posiada wiele aktywności:
-runningActivity
-cyclingActivity 
-walkingActivity 
będą nadpisywały metody CalculateCalories() gdzie będzie się zmieniał współczynnik używany do liczenia spalonych kalorii, dodatkowo będą zapisywały np averageSpeed-średnią prędkość czy steps-liczbe kroków.
activityAnalyzer - klasa odpowiadająca wyłącznie za analizę danych z metodami totalDistance(), totalCalories(), findLongestActivity()
