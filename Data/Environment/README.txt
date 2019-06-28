This Floder contain generated data and figures of indoor scenes and walking trajectories of about 1000 house.
The Framework of this Floder is show in following:

--Data/Environment/
  --Hash_number(0-7)
    --subFolder_name1
      --subFolder_name2
        --Figure
          --.png
        --.json
        --.csv
  --Content.json
  --Statistic.json

We classify the houses by the furniture in them. Different furniture correspond to different Hash_number and subFolder_name1.
For the Hash number: 0 means no Kitchen Stove, no Wardrobe, and no Sofa
                     1 means have Kitchen Stove, no Wardrobe, and no Sofa
                     2 means no Kitchen Stove, have Wardrobe, and no Sofa
                     3 means have Kitchen Stove, have Wardrobe, and no Sofa
                     4 means no Kitchen Stove, no Wardrobe, and have Sofa
                     5 means have Kitchen Stove, no Wardrobe, and have Sofa
                     6 means no Kitchen Stove, have Wardrobe, and have Sofa
                     7 means have Kitchen Stove, have Wardrobe, and have Sofa

subFolder_name1 details all furniture inside the house.
Any house must have Bed, may have Wardrobe, Desk-Chair set, Sofa-TV set, Dinner Table set, Kitchen Stove, Cupboard
                                  Refrigerator, Wash Machine, Trash Bin
If a house have all of them, its subFolder_name1 is WARDeSoDTAKSCBRFAWMTB; 
if a house has no Sofa_TV set and Cupboard, its subFolder_name1 is WARDe00DTAKS00RFAWMTB;

subFolder_name2 details the shape, size of the house.

All generated data is record by .json and .csv files.
For example, Semantic.json record the floorplan, Height_Function.json record the height function.
             Discomfortable_value.csv record the É÷(x), XXX_distance.csv record the LTJ1 function.
             Human_path.function record walking trajectories.

All corresponding figure is in the Figure Floder.
For example, Layout.png is the floorplan, Height_Function.png show the 3D indoor scene
             Discomfortable_value.png show the field of É÷(x), XXX_distance.png show the field of LTJ1 function.
             Human_path[Travel pattern][Start][Destination].png show the walking trajectory.