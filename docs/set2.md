```js
import * as d3 from "npm:d3";

import { FileAttachment } from "npm:@observablehq/stdlib";

let finalCountsMap = new Map();
```

```js
const Brain_r1 = FileAttachment("/releases/Release 1/Brain_V1.csv");
const Heart_r1 = FileAttachment("/releases/Release 1/Heart_V1.csv");
const Blood_Pelvis_r1 = FileAttachment("/releases/Release 1/Blood_Pelvis_V1.csv");
const Large_Intestine_r1 = FileAttachment("/releases/Release 1/IntestineLarge_V1.csv");
const Kidney_r1 = FileAttachment("/releases/Release 1/Kidney_V1.csv");
const Lung_r1 = FileAttachment("/releases/Release 1/Lung_V1.csv");
const Lymph_Node_r1 = FileAttachment("/releases/Release 1/Lymph_Node_V1.csv");
const Skin_r1 = FileAttachment("/releases/Release 1/Skin_V1.csv");
const Spleen_r1 = FileAttachment("/releases/Release 1/Spleen_V1.csv");
const Thymus_r1 = FileAttachment("/releases/Release 1/Thymus_V1.csv");
const Vasculature_r1 = FileAttachment("/releases/Release 1/Vasculature_V1.csv");
const Blood_Pelvis_r2 = FileAttachment("/releases/Release 2/Blood_Pelvis_V2.csv");
const Blood_Vasculature_r2 = FileAttachment("/releases/Release 2/Blood_Vasculature_V2.csv");
const BoneMarrow_Pelvis_r2 = FileAttachment("/releases/Release 2/BoneMarrow_Pelvis_V2.csv");
const Brain_r2 = FileAttachment("/releases/Release 2/Brain_V2.csv");
const Eye_r2 = FileAttachment("/releases/Release 2/Eye_V2.csv");
const Fallopian_Tube_r2 = FileAttachment("/releases/Release 2/Fallopian_Tube_V2.csv");
const Heart_r2 = FileAttachment("/releases/Release 2/Herat_V2.csv");
const Kidney_r2 = FileAttachment("/releases/Release 2/Kidney_V2.csv");
const Knee_r2 = FileAttachment("/releases/Release 2/Knee_V2.csv");
const Large_Intestine_r2 = FileAttachment("/releases/Release 2/Large_Intestine_V2.csv");
const Liver_r2 = FileAttachment("/releases/Release 2/Liver_V2.csv");
const Lung_r2 = FileAttachment("/releases/Release 2/Lung_V2.csv");
const Lymph_Node_r2 = FileAttachment("/releases/Release 2/Lymph_Node_V2.csv");
const Lymph_Vasculature_r2 = FileAttachment("/releases/Release 2/Lymph_Vasculature_V2.csv");
const Ovary_r2 = FileAttachment("/releases/Release 2/Ovary_V2.csv");
const Pancreas_r2 = FileAttachment("/releases/Release 2/Pancreas_V2.csv");
const Peripheral_Nervous_System_r2 = FileAttachment("/releases/Release 2/Peripheral_Nervous_System_V2.csv");
const Prostate_r2 = FileAttachment("/releases/Release 2/Prostate_V2.csv");
const Skin_r2 = FileAttachment("/releases/Release 2/Skin_V2.csv");
const Small_Intestine_r2 = FileAttachment("/releases/Release 2/Small_Intestine_V2.csv");
const Spleen_r2 = FileAttachment("/releases/Release 2/Spleen_V2.csv");
const Thymus_r2 = FileAttachment("/releases/Release 2/Thymus_V2.csv");
const Ureter_r2 = FileAttachment("/releases/Release 2/Ureter_V2.csv");
const Urinary_Bladder_r2 = FileAttachment("/releases/Release 2/Urinary_Bladder_V2.csv");
const Uterus_r2 = FileAttachment("/releases/Release 2/Uterus_V2.csv");
const Blood_Pelvis_r3 = FileAttachment("/releases/Release 3/Blood_Pelvis_V3.csv");
const Blood_Vasculature_r3 = FileAttachment("/releases/Release 3/Blood_Vasculature_V3.csv");
const BoneMarrow_Pelvis_r3 = FileAttachment("/releases/Release 3/BoneMarrow_Pelvis_V3.csv");
const Brain_r3 = FileAttachment("/releases/Release 3/Brain_V3.csv");
const Eye_r3 = FileAttachment("/releases/Release 3/Eye_V3.csv");
const Fallopian_Tube_r3 = FileAttachment("/releases/Release 3/Fallopian_Tube_V3.csv");
const Heart_r3 = FileAttachment("/releases/Release 3/Herat_V3.csv");
const Kidney_r3 = FileAttachment("/releases/Release 3/Kidney_V3.csv");
const Knee_r3 = FileAttachment("/releases/Release 3/Knee_V3.csv");
const Large_Intestine_r3 = FileAttachment("/releases/Release 3/Large_Intestine_V3.csv");
const Liver_r3 = FileAttachment("/releases/Release 3/Liver_V3.csv");
const Lung_r3 = FileAttachment("/releases/Release 3/Lung_V3.csv");
const Lymph_Node_r3 = FileAttachment("/releases/Release 3/Lymph_Node_V3.csv");
const Lymph_Vasculature_r3 = FileAttachment("/releases/Release 3/Lymph_Vasculature_V3.csv");
const Ovary_r3 = FileAttachment("/releases/Release 3/Ovary_V3.csv");
const Pancreas_r3 = FileAttachment("/releases/Release 3/Pancreas_V3.csv");
const Placenta_r3 = FileAttachment("/releases/Release 3/Placenta_Full_Term_V3.csv");
const Prostate_r3 = FileAttachment("/releases/Release 3/Prostate_V3.csv");
const Skin_r3 = FileAttachment("/releases/Release 3/Skin_V3.csv");
const Small_Intestine_r3 = FileAttachment("/releases/Release 3/Small_Intestine_V3.csv");
const Spleen_r3 = FileAttachment("/releases/Release 3/Spleen_V3.csv");
const Thymus_r3 = FileAttachment("/releases/Release 3/Thymus_V3.csv");
const Ureter_r3 = FileAttachment("/releases/Release 3/Ureter_V3.csv");
const Urinary_Bladder_r3 = FileAttachment("/releases/Release 3/Urinary_Bladder_V3.csv");
const Uterus_r3 = FileAttachment("/releases/Release 3/Uterus_V3.csv");
const Blood_Pelvis_r4 = FileAttachment("/releases/Release 4/blood_pelvis_V4.csv");
const Blood_Vasculature_r4 = FileAttachment("/releases/Release 4/blood_vasculature_V4.csv");
const BoneMarrow_Pelvis_r4 = FileAttachment("/releases/Release 4/bonemarrow_pelvis_V4.csv");
const Brain_r4 = FileAttachment("/releases/Release 4/Brain_V4.csv");
const Eye_r4 = FileAttachment("/releases/Release 4/eye_V4.csv");
const Fallopian_Tube_r4= FileAttachment("/releases/Release 4/Fallopian_Tube_V4.csv");
const Heart_r4 = FileAttachment("/releases/Release 4/Herat_V4.csv");
const Kidney_r4 = FileAttachment("/releases/Release 4/Kidney_V4.csv");
const Knee_r4 = FileAttachment("/releases/Release 4/Knee_V4.csv");
const Large_Intestine_r4 = FileAttachment("/releases/Release 4/large-intestine_V4.csv");
const Liver_r4 = FileAttachment("/releases/Release 4/Liver_V4.csv");
const Lung_r4 = FileAttachment("/releases/Release 4/Lung_V4.csv");
const Lymph_Node_r4 = FileAttachment("/releases/Release 4/Lymph_Node_V4.csv");
const Lymph_Vasculature_r4 = FileAttachment("/releases/Release 4/lymph-vasculature_V4.csv");
const Ovary_r4 = FileAttachment("/releases/Release 4/Ovary_V4.csv");
const Pancreas_r4 = FileAttachment("/releases/Release 4/pancreas_V4.csv");
const Peripheral_Nervous_System_r4 = FileAttachment("/releases/Release 4/Peripheral_Nervous_System_V4.csv");
const Placenta_r4 = FileAttachment("/releases/Release 4/Placenta_Full_Term_V4.csv");
const Prostate_r4 = FileAttachment("/releases/Release 4/Prostate_V4.csv");
const Skin_r4 = FileAttachment("/releases/Release 4/Skin_V4.csv");
const Small_Intestine_r4 = FileAttachment("/releases/Release 4/small-intestine_V4.csv");
const Spleen_r4 = FileAttachment("/releases/Release 4/spleen_V4.csv");
const Thymus_r4 = FileAttachment("/releases/Release 4/thymus_V4.csv");
const Ureter_r4= FileAttachment("/releases/Release 4/Ureter_V4.csv");
const Urinary_Bladder_r4 = FileAttachment("/releases/Release 4/Urinary_Bladder_V4.csv");
const Uterus_r4 = FileAttachment("/releases/Release 4/Uterus_V4.csv");
const Blood_Vasculature_r5 = FileAttachment("/releases/Release 5/blood-vasculature_V5.csv");
const Brain_r5 = FileAttachment("/releases/Release 5/Brain_V5.csv");
const Bronchus_r5 = FileAttachment("/releases/Release 5/bronchus_V5.csv");
const Eye_r5 = FileAttachment("/releases/Release 5/eye_V5.csv");
const Kidney_r5 = FileAttachment("/releases/Release 5/kidney_V5.csv");
const Lung_r5 = FileAttachment("/releases/Release 5/lung_V5.csv");
const Lymph_Vasculature_r5 = FileAttachment("/releases/Release 5/lymph-vasculature_V5.csv");
const Muscular_System_r5 = FileAttachment("/releases/Release 5/muscular-system_V5.csv");
const Skeleton_r5 = FileAttachment("/releases/Release 5/skeleton_V5.csv");
const Spinal_Cord_r5 = FileAttachment("/releases/Release 5/spinal-cord_V5.csv");
const Trachea_r5 = FileAttachment("/releases/Release 5/trachea_V5.csv");
const Anatomical_Sysystem_r6 = FileAttachment("/releases/Release 6/anatomical-systems_V6.csv");
const Blood_Vasculature_r6 = FileAttachment("/releases/Release 6/blood-vasculature_V6.csv");
const BoneMarrow_Pelvis_r6 = FileAttachment("/releases/Release 6/bone-marrow_V6.csv");
const Brain_r6 = FileAttachment("/releases/Release 6/Brain_V6.csv");
const Heart_r6 = FileAttachment("/releases/Release 6/Heart_V6.csv");
const Fallopian_Tube_r6 = FileAttachment("/releases/Release 6/fallopian-tube_V6.csv");
const Kidney_r6 = FileAttachment("/releases/Release 6/kidney_V6.csv");
const Knee_r6 = FileAttachment("/releases/Release 6/knee_V6.csv");
const Liver_r6 = FileAttachment("/releases/Release 6/liver_V6.csv");
const Lung_r6 = FileAttachment("/releases/Release 6/lung_V6.csv");
const Lymph_Node_r6 = FileAttachment("/releases/Release 6/lymph-node_V6.csv");
const Lymph_Vasculature_r6 = FileAttachment("/releases/Release 6/lymph-vasculature_V6.csv");
const Bronchus_r6 = FileAttachment("/releases/Release 6/main-bronchus_V6.csv");
const Muscular_System_r6 = FileAttachment("/releases/Release 6/muscular-system_V6.csv");
const Musculoskeletal_r6 = FileAttachment("/releases/Release 6/musculoskeletal_different_V6.csv");
const Tonsil_r6 = FileAttachment("/releases/Release 6/palatine-tonsil_V6.csv");
const Pancreas_r6 = FileAttachment("/releases/Release 6/pancreas_V6.csv");
const Peripheral_Nervous_System_r6 = FileAttachment("/releases/Release 6/peripheral-nervous-system_V6.csv");
const Placenta_r6 = FileAttachment("/releases/Release 6/placenta_V6.csv");
const Prostate_r6 = FileAttachment("/releases/Release 6/prostate_V6.csv");
const Skeleton_r6 = FileAttachment("/releases/Release 6/skeleton_V6.csv");
const Skin_r6 = FileAttachment("/releases/Release 6/skin_V6.csv");
const Thymus_r6 = FileAttachment("/releases/Release 6/thymus_V6.csv");



// const loopArr = [
//   { organ: "Brain", releases: [ Brain_r1, Brain_r2, Brain_r3, Brain_r4, Brain_r5, Brain_r6 ] },
//   { organ: "Lymph_Node", releases: [Lymph_Node_r1, Lymph_Node_r2,Lymph_Node_r3, Lymph_Node_r4, Lymph_Node_r6 ] },
//   { organ: "Blood_Pelvis", releases: [Blood_Pelvis_r1, Blood_Pelvis_r2, Blood_Pelvis_r3, Blood_Pelvis_r4 ] },
//   { organ: "Heart", releases: [Heart_r1, Heart_r2, Heart_r3, Heart_r4, Heart_r6] },
//   { organ: "Small_Intestine", releases:[Small_Intestine_r2, Small_Intestine_r3, Small_Intestine_r4 ]},
//   { organ: "Kidney",releases: [Kidney_r1,Kidney_r2, Kidney_r3, Kidney_r4, Kidney_r5, Kidney_r6]},
//   { organ: "Lung",releases:[Lung_r1, Lung_r2, Lung_r3, Lung_r4, Lung_r5, Lung_r6]},
//   { organ: "Skin",releases:[Skin_r1, Skin_r2, Skin_r3, Skin_r4, Skin_r6]},
//   { organ: "Spleen",releases:[Spleen_r1, Spleen_r2,Spleen_r3, Spleen_r4 ]},
//   { organ: "Thymus",releases:[Thymus_r1, Thymus_r2, Thymus_r3, Thymus_r4, Thymus_r6]},
//   { organ: "Blood_Vasculature",releases:[ Vasculature_r1, Blood_Vasculature_r2, Blood_Vasculature_r3, Blood_Vasculature_r4, Blood_Vasculature_r5, Blood_Vasculature_r6]},
//   { organ: "BoneMarrow_Pelvis",releases: [BoneMarrow_Pelvis_r2, BoneMarrow_Pelvis_r3, BoneMarrow_Pelvis_r4, BoneMarrow_Pelvis_r6]},
//   { organ: "Eye",releases:[Eye_r2, Eye_r3,Eye_r4, Eye_r5]},
//   { organ: "Fallopian_Tube",releases:[Fallopian_Tube_r2, Fallopian_Tube_r3, Fallopian_Tube_r4, Fallopian_Tube_r6]},
//   { organ: "Knee",releases:[Knee_r2, Knee_r3, Knee_r4, Knee_r6]},
//   { organ: "Large_Intestine",releases:[Large_Intestine_r1, Large_Intestine_r2, Large_Intestine_r3,Large_Intestine_r4 ]},
//   { organ: "Liver",releases:[Liver_r2, Liver_r3, Liver_r4, Liver_r6]},
//   { organ: "Ovary",releases:[Ovary_r2, Ovary_r3, Ovary_r4 ]},
//   { organ: "Pancreas",releases:[Pancreas_r2, Pancreas_r3, Pancreas_r4, Pancreas_r6]},
//   { organ: "Peripheral_Nervous_System",releases:[Peripheral_Nervous_System_r2, Peripheral_Nervous_System_r4, Peripheral_Nervous_System_r6]},
//   { organ: "Prostate",releases:[Prostate_r2, Prostate_r3, Prostate_r4, Prostate_r6]},
//   { organ: "Ureter",releases:[Ureter_r2, Ureter_r3, Ureter_r4]},
//   { organ: "Urinary_Ballder",releases:[Urinary_Bladder_r2, Urinary_Bladder_r3, Urinary_Bladder_r4 ]},
//   { organ: "Uterus",releases:[Uterus_r2, Uterus_r3, Uterus_r4]},
//   { organ: "Lymph_Vasculature",releases:[Lymph_Vasculature_r2,Lymph_Vasculature_r3, Lymph_Vasculature_r4, Lymph_Vasculature_r5, Lymph_Vasculature_r6 ]},
//   { organ: "Placenta",releases:[Placenta_r3, Placenta_r4, Placenta_r6]},
//   { organ: "Bronchus",releases:[Bronchus_r5, Bronchus_r6]},
//   { organ: "Muscular_System",releases:[Muscular_System_r5, Muscular_System_r6]},
//   { organ: "Skeleton",releases:[Skeleton_r5, Skeleton_r6]},
//   { organ: "Spinal_Cord",releases:[Spinal_Cord_r5]},
//   { organ: "Trachea",releases:[Trachea_r5]},
//   { organ: "Anatomical_Systems",releases:[Anatomical_Sysystem_r6]},
//   { organ: "Tonsil",releases:[Tonsil_r6]}
// ];

Promise.all(
  loopArr.flatMap((i) => {
    i.releases.map((file) =>
      file.csv({ typed: true }).then((data) => {
        let ct1Count = 0;
        let as1Count = 0;
        let bg1Count = 0;
        let bp1Count = 0;

        for (let i = 0; i < data.length; i++) {
          if (data[i]["CT/1"] && data[i]["CT/1"].trim() !== "") {
            ct1Count++;
          }
          if (data[i]["AS/1"] && data[i]["AS/1"].trim() !== "") {
            as1Count++;
          }
          if (data[i]["BGene/1"] && data[i]["BGene/1"].trim() !== "") {
            bg1Count++;
          }
          if (data[i]["BProtein/1"] && data[i]["BProtein/1"].trim() !== "") {
            bp1Count++;
          }
        }

        if (finalCountsMap.has(i.organ)) {
          let currentData = finalCountsMap.get(i.organ);
          currentData.ct1 += ct1Count;
          currentData.as1 += as1Count;
          currentData.bg1 += bg1Count;
          currentData.bp1 += bp1Count;
        } else {
          finalCountsMap.set(i.organ, {
            ct1: ct1Count,
            as1: as1Count,
            bg1: bg1Count,
            bp1: bp1Count,
          });
        }
      })
    );
  })
).then(() => {
  console.log(finalCountsMap);
});
```
<div>
  <p>Plot</p>
</div>

<div style="display: flex;">
  <!-- Graph -->
  <div id="graph" style="flex: 1;"></div>

  <!-- Legend -->
  <div style="margin-top: 20px; margin-left: 20px;">
    <div style="display: flex; align-items: center;">
      <svg width="10" height="10">
        <rect width="10" height="10" fill="red"></rect>
      </svg>
      <div style="margin-left: 5px;">CT/1</div>
    </div>
    <div style="display: flex; align-items: center;">
      <svg width="10" height="10">
        <rect width="10" height="10" fill="blue"></rect>
      </svg>
      <div style="margin-left: 5px;">AS/1</div>
    </div>
    <div style="display: flex; align-items: center;">
      <svg width="10" height="10">
        <rect width="10" height="10" fill="green"></rect>
      </svg>
      <div style="margin-left: 5px;">BProtein/1</div>
    </div>
    <div style="display: flex; align-items: center;">
      <svg width="10" height="10">
        <rect width="10" height="10" fill="yellow"></rect>
      </svg>
      <div style="margin-left: 5px;">BGene/1</div>
    </div>
  </div>
</div>

```js
// Code for plotting graph
// Assuming `organCountsMap` is your Map object with organ counts
const dataForPlotting = Array.from(finalCountsMap, ([organ, counts]) => ({
  organ: organ, // this is the x-axis
  ct1: counts.ct1,
  as1: counts.as1,
  bp1: counts.bp1,

  bg1: counts.bg1,
}));

// Now you can use Plot.plot to generate the graph
function drawChart() {
  return Plot.plot({
    marginTop: 40,        // Add margin to accommodate x-axis labels
    marginBottom: 150,     // Add margin to accommodate x-axis labels and ticks
    marginLeft: 80,       // Add margin to accommodate y-axis labels and ticks
    marginRight: 5, 
    // style: "overflow: visible;",
    y: { grid: true },
    x: {
    
      // type: "linear",
      domain: ["Brain", "Lymph_Node", "Blood_Pelvis","Heart","Small_Intestine","Kidney","Lung","Skin","Spleen","Thymus","Blood_Vasculature","BoneMarrow_Pelvis","Eye","Fallopian_Tube","Knee","Large_Intestine","Liver","Ovary","Pancreas","Peripheral_Nervous_System","Prostate","Ureter","Urinary_Ballder","Uterus","Lymph_Vasculature","Placenta","Bronchus","Muscular_System","Skeleton","Spinal_Cord","Trachea","Anatomical_Systems","Tonsil"],
      // label:"Organ",


      tickRotate:-40,
      tickCount: 10,
      LabelOffset:-10000,
      padding: 0.00001 // Set the domain to the list of organs
    },


    marks: [
      // One line for each category of counts. Assuming 'dataForPlotting' is structured correctly.
      Plot.line(dataForPlotting, { x: "organ", y: "ct1", stroke: "red" }),
      Plot.line(dataForPlotting, { x: "organ", y: "as1", stroke: "blue" }),
      Plot.line(dataForPlotting, { x: "organ", y: "bp1", stroke: "green" }),
      Plot.line(dataForPlotting, { x: "organ", y: "bg1", stroke: "yellow" }),
      Plot.dot(dataForPlotting, { x: "organ", y: "ct1", fill: "red" }),
      Plot.dot(dataForPlotting, { x: "organ", y: "as1", fill: "blue" }),

      Plot.dot(dataForPlotting, { x: "organ", y: "bp1", fill: "green" }),




      Plot.dot(dataForPlotting, { x: "organ", y: "bg1", fill: "orange" }),
    ],
  });
  svg.selectAll('.dot')
    .on('mouseover', () => {

      console.log('hi');
    });

  return svg;
  


}
```
<div>
  <div>${drawChart()}</div>
</div> 