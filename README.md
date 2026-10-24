# RoadScan
Multimodal 3D road inspection: YOLO + SAM + Depth Anything + ByteTrack


---

## Week 1 — Smoke test (current)

Verified that all three foundation models run end-to-end on a single sample image:

- ✅ PyTorch 2.x + CUDA verified on Colab T4 (15.6 GB VRAM)
- ✅ YOLO11n loaded from `yolo11n.pt`, inference runs
- ✅ SAM 2 tiny checkpoint (`sam2_hiera_tiny.pt`) downloaded, `SAM2ImagePredictor` works with box prompt
- ✅ Depth Anything V2 Small loaded from Hugging Face, depth inference runs
- ✅ Three-model pipeline runs end-to-end on one image

See: [`notebooks/00_smoke_test.ipynb`](./notebooks/00_smoke_test.ipynb)

---

## Roadmap

- [x] Week 1 — Environment setup + smoke test
- [ ] Week 2 — Baseline YOLO11n training on RDD2022
- [ ] Week 3 — Error analysis in FiftyOne on BDD100K scenes
- [ ] Week 4 — SAM 2 + Depth Anything V2 integration with mm calibration
- [ ] Week 5 — ByteTrack cross-frame tracking
- [ ] Week 6 — Ablations (YOLO11n vs s, with/without SAM 2, with/without ByteTrack)
- [ ] Week 7 — ONNX export + INT8 quantization + benchmark
- [ ] Week 8 — FastAPI service + Docker container
- [ ] Week 9 — GIS heatmap overlay (Folium + OpenStreetMap)
- [ ] Week 10 — Hugging Face Spaces deployment + 1-page writeup

---

## Author

**Abdul Raheem** — BS Computer Science, NUST Islamabad (graduating 2027)

📧 abdurraheem6335@gmail.com

---

## License

MIT
