[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=drLKeen/matlabfeatures25a)

<a id="TMP_171f"></a>

# What's New in MATLAB: 2025a
<!-- Begin Toc -->

## Table of Contents
&emsp;[Explore & Design](#TMP_7317)
 
&emsp;&emsp;[User Interface](#TMP_4e34)
 
&emsp;&emsp;[Improved Live Editor and Live Script](#TMP_4934)
 
&emsp;&emsp;[MATLAB Copilot](#TMP_830d)
 
&emsp;[Share & Deploy](#TMP_651c)
 
&emsp;&emsp;[App Designer (+Dark Mode)](#TMP_30e5)
 
&emsp;&emsp;[Source Control Integration](#TMP_5568)
 
<!-- End Toc -->
<a id="TMP_745e"></a>
```matlab
airq = readtable('madrid_2018.csv')
```


| |date|BEN|CH4|CO|EBE|NMHC|NO|NO_2|NOx|O_3|PM10|PM25|SO_2|TCH|TOL|station|
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|1|2018-03-01 01:00:00|NaN|NaN|0.3000|NaN|NaN|1|29|31|NaN|NaN|NaN|2|NaN|NaN|28079004|
|2|2018-03-01 01:00:00|0.5000|1.3900|0.3000|0.2000|0.0200|6|40|49|52|5|4|3|1.4100|0.8000|28079008|
|3|2018-03-01 01:00:00|0.4000|NaN|NaN|0.2000|NaN|4|41|47|NaN|NaN|NaN|NaN|NaN|1.1000|28079011|
|4|2018-03-01 01:00:00|NaN|NaN|0.3000|NaN|NaN|1|35|37|54|NaN|NaN|NaN|NaN|NaN|28079016|


```matlab
airq = sortrows(airq,"date","ascend");
```
<a id="TMP_7317"></a>

# Explore & Design
<a id="TMP_4e34"></a>

## User Interface
```matlab
DarkMode = true;
NewPanels = true; % 
```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Debugger, Source Control, Project, Save Current Layout

```matlab
VarEditWin = true; % Variable Editor window
FigureWin = true; % New Figure Window
```
<a id="TMP_4934"></a>

## Improved Live Editor and Live Script

![image_0.png](./WhatsNew25a_media/image_0.png)

```matlab
apptaskw = true;% More apps, tasks, and workflows, 

vids = true;% Embedded videos
plaintext = true;% Live Scripts as .m - plain text!
fcnmiddle = true;% Functions in middle of script
mdgen = true;% Markdown generation
```
<a id="TMP_830d"></a>

## MATLAB Copilot
```matlab
Copilot = true;
```

<a id="TMP_651c"></a>

# Share & Deploy
<a id="TMP_30e5"></a>

## App Designer (+Dark Mode)
```matlab
Standalone = false;% Standalone Apps
AIO = false;% All In One: App, Toolbox, Project
```
<a id="TMP_5568"></a>

## Source Control Integration
```matlab
GitHub = false; % Direct GitHub integrations
MLO = false; % Open in MATLAB Online 

```

```matlab
% Python code input
pycode = [...
"import numpy as np",...
"",...
"x = 42",...
"var = np.sqrt(42)",...
"",...
"print(var)"...
];

try
    [x, var] = pyrun(pycode, ...
         [ "x" "var" ])
catch ME7
    % Clear temporary variables from workspace and from Python
    clear pycode;
    rethrow(ME7)
end
```

```matlabTextOutput
Error using > (line 1)
Python Error: ModuleNotFoundError: No module named 'numpy'
```

```matlab

% Clear temporary variables from workspace and from Python
clear pycode;
```

https://www.mathworks.com/products/matlab\-online/git.html


[Example 1](https://www.mathworks.com/matlabcentral/fileexchange/160986-precipitation-variability-analysis-matlab)


[Example 2](https://github.com/mathworks/Seismic-HAzard-Parameters-Evaluation-Interface-SHAppE)

