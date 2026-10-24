# Benchmark tables (machine-readable)

CSV versions of the tables in the survey. Every value is the one **reported by the original authors**; see the survey for full protocols.

| File | Content | Protocol notes |
|---|---|---|
| `coco_realtime_yolo.csv` | COCO val2017 AP, params, GFLOPs, latency of YOLOv8–YOLO26 | 640×640; latency on NVIDIA T4, TensorRT FP16, batch 1. YOLO26 AP given as "with NMS / NMS-free". |
| `coco_realtime_detr.csv` | Same for RT-DETR, RT-DETRv2, D-FINE, DEIM, DEIMv2, LW-DETR, RF-DETR | `PT`: O365 = Objects365 pre-training; DINO = DINOv2/v3 backbone pre-training. |
| `lvis_zeroshot_ovd.csv` | Zero-shot LVIS-minival AP / AP_r and COCO AP of open-vocabulary detectors | Fixed AP unless noted. `*` FPS values are from different GPUs/papers and are not directly comparable. |
| `mllm_f1.csv` | F1@IoU0.5 of MLLM detectors (from the Rex-Omni paper) | Not comparable with AP. |
| `anomaly_auroc.csv` | Image-level AUROC on MVTec AD / VisA | Zero-shot values as compiled in AnomalyCLIP. |
| `yolo_genealogy.csv` | Architecture, assignment and loss of each YOLO version | — |
| `datasets_general.csv`, `datasets_applications.csv` | Benchmark datasets | — |
| `edge_hardware.csv` | Edge accelerators (vendor specifications) | Peak throughput as quoted by vendors. |
| `mllm_agentic_systems.csv` | MLLM-based and agentic detection systems | D = direct coordinates, RL = RL-tuned, T = tool use. |
| `survey_comparison.csv` | Coverage comparison with other surveys | yes / partial / no |

`-` means not reported in the cited source.
