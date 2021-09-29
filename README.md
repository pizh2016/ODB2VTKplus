# ODB2VTKplus test_version
   This Python script is released with the paper: LIU Qing-bin, PAN Mao, LIU Jie, GUO Yan-jun, ZHANG Xiao-shuang, YAO Jian-peng, LI Fang-yu. ParaView Visualization and Virtual Reality of Output of Finite Element Analysis in Abaqus[J/OL]. Rock and Soil Mechanics,2019(12):1-9[2019-05-25]. https://doi.org/10.16285/j.rsm.2018.1794. Please cite it if the script is used in your reports/papers.

   We suggest the samples from https://github.com/Liujie-SYSU/odb2vtk/tree/master/Samples to learn the script.

   Note: Some modifications to script is necessary when handle different mission.

# ODB2VTKplus update 1.0.1 (Support Multiple Instances)

## Python script "ODB2VTK-Multiple.py" is released. 
   Most functions inherit from "ODB2VTK+.py" . This version Support Multiple Instances if odb file contains more than 1 instance, and cteate .vtu file for each instance(use frame.fieldOutputs[variable_name].getSubset(region=instance_region), instance_region = odb.rootAssembly.instances[instancename]).


## fixed some config problems:
   auto create vtk_path 
   if no scalar or vector to be read in odb, use " scalar = '' ", free to select variable(discard order)
   optimize write function, improve loop efficiency for big model

   You can test from Samples/xxx.odb with Abaqus version >= 2019. For more infomation, please sent your email to pizh12thu@foxmail.com, or go to https://www.zhihu.com/people/pizh12thu
