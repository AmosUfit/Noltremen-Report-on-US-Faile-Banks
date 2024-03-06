# Noltremen-Report-on-US-Faile-Banks
Power BI Report on FDIC Failed banks in the US created by Noltremen

## Data Source
https://www.fdic.gov/bank/individual/failed/banklist.csv
Data taken from web and loaded therefrom

## Data Transform Process
1. Data loaded taken from the web
2. Transformation of data by reducing the columns found not needed for the visualization -
3. Created a new column, "City State" through DAX function
4. Loaded Dataset after transformation

## DAX Written for Date Table
1. Calendar = Calendarauto()
2. Year = Year('Calendar'[Date])
3. Month Number = Month('Calendar'[Date])
4. Month Name = Format('Calendar'[Date], "mmmm")
5. Click "Mark as Date Table"

## DAX Written for New Measure
1. City State = Marge Columns (City & State) - City State = Measure by Example

## Visuals & Insights
1. Visual to check number of failed banks by State - 
2. Visual to Check the state with the highest failed banks - **State with Highest failed banks is Georgia**
3. Visual to check total failed banks by months
4. Visuals to view the highest month with failed banks - **Month with highest failed banks is July**
5. Visuals to view failed banks by year - **Year with highest failed bank is 2010**
6. Slicer (Play Axis) to automatically slice information on all the visuals by year

## Tooltip
1. Tooltip created for total number of banks and state information using map
2. When hovering on the visual with state information, tooltips display the information boldly

## Dashboard Visualization
<img width="506" alt="image" src="https://github.com/AmosUfit/Noltremen-Report-on-US-Faile-Banks/assets/88596615/60cfa2a1-4aa0-4195-a653-747cdb105be9">

## Tooltip Visualization
<img width="514" alt="image" src="https://github.com/AmosUfit/Noltremen-Report-on-US-Faile-Banks/assets/88596615/25e3f5ea-df8f-4637-9c3b-3ad05397c3d4">

