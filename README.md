# AICP Quantum Computing Simulator

**AI designed this project based on the AICP protocol, offering a new approach to unifying quantum computing operations. Experts welcome to dive deeper.**

[→ View the full experiment](./experiment.md)

---

## Why It Matters

- **Quantum gates are not classes. They're Envelop queries.** Qiskit uses `HadamardGate` classes. Cirq uses `Gate` interfaces. AICP sends a single `gate/h` Envelop and gets a matrix back. Quantum mechanics reduced to message flow.

- **Circuit compilation is Envelop translation.** You send logical gates `["H", "CNOT", "X"]`. The quantum chip replies with physical pulses `["pulse_H", "pulse_CNOT", "pulse_X"]`. Compilation is no longer a complex optimization framework—it's an input-output Envelop transformation.

- **VQE is Envelop round-trips.** The classical optimizer sends an Envelop to the quantum chip → the chip measures and returns the energy value → the optimizer adjusts parameters and sends again. Quantum-classical hybrid computing becomes a message dialogue.

- **Any quantum processor can plug in.** This isn't a Qiskit replacement—it's more fundamental. Any quantum chip that understands AICP Envelops—IBM, Google, Rigetti—can be programmed with the same set of messages. Vendor lock-in, dissolved by a protocol.

- **AI generated the entire system from the protocol alone.** No quantum computing textbooks. No Qiskit source code. No Cirq documentation. The AI read only the AICP protocol and generated qubit management, standard quantum gates, a circuit compiler, noise simulation, Shor code and Surface code error correction, and a VQE hybrid interface.

---

## What This Solves

**1. Vendor lock-in.** A circuit written in Qiskit cannot run directly on Google's quantum hardware. AICP's message format is universal—any chip that understands the nine-field Envelop can execute any quantum program.

**2. Quantum software stack complexity.** Traditional frameworks have class inheritance, abstract interfaces, backend adaptation layers. AICP flattens all of this into Envelop paths. Want a new quantum gate? Add a new path. No architecture changes needed.

**3. AI cannot generate quantum programs.** Qiskit and Cirq APIs are designed for humans—object-oriented, multi-layered abstractions. AICP's API is nine JSON fields. AI can understand it directly. AI can generate it directly.

---

> **Open question:** Can the operating system layer of quantum computing really be defined by a nine-field message protocol? Or is there necessary complexity in Qiskit and Cirq that we haven't yet recognized?

---

## Related Projects

| Project | Description |
|---|---|
| [aicp-eat](https://github.com/woozheng/aicp-eat) | Core engine / 核心引擎 |
| [aicp-os-kernel](https://github.com/woozheng/aicp-os-kernel) | Microkernel OS / 微内核操作系统 |
| [aicp-quantum](https://github.com/woozheng/aicp-quantum) | Quantum computing / 量子计算 |
| [aicp-protein](https://github.com/woozheng/aicp-protein) | Protein folding / 蛋白质折叠 |
| [aicp-llm-trainer](https://github.com/woozheng/aicp-llm-trainer) | LLM training / 大模型训练 |
| [aicp-riemann](https://github.com/woozheng/aicp-riemann) | Riemann Hypothesis / 黎曼猜想 |
| [aicp-ai-chip](https://github.com/woozheng/aicp-ai-chip) | AI chip design / AI 芯片设计 |
| [aicp-raw-experiments](https://github.com/woozheng/aicp-raw-experiments) | Raw experiments / 原始实验 |

---

## License

MIT · See [LICENSE](https://github.com/woozheng/aicp-eat/blob/main/LICENSE)