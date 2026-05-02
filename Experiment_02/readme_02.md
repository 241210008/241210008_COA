
# Experiment 2

## Design of 4-bit Ripple Carry Adder and Analysis of Propagation Delay

---

##  Objective

The purpose of this experiment is to design and simulate a 4-bit Ripple Carry Adder (RCA) using basic logic gates in Logisim Evolution, and to study the propagation delay involved in carry generation and output calculation. The experiment helps in understanding how carry signals move across multiple stages and how this influences the overall performance of the circuit.

---

## Background Study

A Ripple Carry Adder is a combinational circuit used for adding binary numbers of multiple bits. It is formed by connecting several full adders in sequence, where the carry output of one full adder becomes the carry input of the next. In a 4-bit RCA, four full adders are connected to perform the addition of two 4-bit numbers along with an initial carry input.

Each full adder produces a sum and a carry output based on its inputs. One limitation of this design is the delay caused due to the step-by-step propagation of the carry from the least significant bit (LSB) to the most significant bit (MSB). The final result is available only after the carry passes through all stages, which makes the circuit slower as the number of bits increases.

---

## Circuit Description

In this experiment, a 4-bit Ripple Carry Adder was constructed using basic logic gates such as AND, OR, and XOR. Each stage functions as a full adder, taking two input bits along with a carry input to produce a sum and a carry output. The carry output from each stage is connected to the next stage, forming a sequential chain.

The circuit was simulated in Logisim, where various input combinations were applied to verify the correctness of the outputs. The carry propagation through each stage was carefully observed, demonstrating the delay in producing the final output.

---

##  Circuit Diagram


[Lab Implentation(Logisim) of Experiment](https://github.com/241210047/241210047_COA/blob/main/Experiment_02/Lab_02.png)


---

## 🔍 Observations

The simulation showed that the sum outputs were generated correctly for all input combinations. However, it was observed that the carry signal propagates sequentially from one stage to another, introducing a delay in the final output. The delay increases with the number of bits, as each stage must wait for the carry from the previous stage before producing its result.

---

## ⏱️ Propagation Delay Analysis

The total propagation delay of a Ripple Carry Adder is directly proportional to the number of bits. In a 4-bit RCA, the worst-case delay occurs when the carry must propagate through all four stages. This delay can be expressed as the sum of delays of individual full adders, making the circuit slower compared to more advanced adders like carry look-ahead adders.

---

## 🎯 Result

The 4-bit Ripple Carry Adder was successfully designed and simulated using Logisim Evolution. The outputs were verified and found to be correct. The experiment clearly demonstrated the concept of carry propagation and highlighted the impact of propagation delay on circuit performance.

---

## 📚 Conclusion

This experiment helped in understanding the working of multi-bit addition using Ripple Carry Adders and the effect of carry propagation on computation speed. It also highlighted the limitations of RCA in terms of delay, emphasizing the importance of more advanced adder designs for high-speed applications.

