# Microeconomics 2026

*Introductory + Intermediate Microeconomics — USYD-aligned self-study course*

## About This Course

This course covers introductory and intermediate microeconomics following the structure of USYD's ECON1001 and ECOS2001. Designed for two learners: one applying microeconomics to professional work, and one undergraduate student currently attending ECON1001 at USYD.

**Duration:** 180 days × 30 minutes per day (~90 hours total)  
**Level:** Introductory (Modules 01–12, 63 lessons) + Intermediate (Modules 13–21, 48 lessons) — **111 lessons total**

## How to Use This Course

1. Work through modules in order — each lesson takes approximately 30 minutes
2. Complete the practice prompts at the end of each lesson before moving on
3. Use the search bar (top right) to find any topic quickly

## Course Structure

| Module | Topic | Lessons |
|--------|-------|---------|
| [M01](modules/module-01/M01.L01-what-is-economics-scarcity-choice.md) | Introduction: Scarcity, Choice, and the Economic Method | 5 |
| [M02](modules/module-02/M02.L01-demand-curve-law-of-demand.md) | Demand and Willingness to Pay | 5 |
| [M03](modules/module-03/M03.L01-production-function-total-average-marginal-product.md) | Production and Costs | 5 |
| [M04](modules/module-04/M04.L01-supply-curve-law-of-supply.md) | Supply and Market Equilibrium | 6 |
| [M05](modules/module-05/M05.L01-consumer-surplus-concept-calculation.md) | Economic Surplus and Elasticity | 6 |
| [M06](modules/module-06/M06.L01-market-structures-overview-four-models.md) | Market Equilibrium and Perfect Competition | 5 |
| [M07](modules/module-07/M07.L01-monopoly-sources-market-power-barriers-entry.md) | Monopoly | 6 |
| [M08](modules/module-08/M08.L01-strategic-interaction-game-theory-basics.md) | Game Theory and Oligopoly | 5 |
| [M09](modules/module-09/M09.L01-price-ceilings-rent-control-shortages.md) | Price Regulation, Taxes, and Subsidies | 5 |
| [M10](modules/module-10/M10.L01-externalities-negative-positive.md) | Externalities and Market Failure | 5 |
| [M11](modules/module-11/M11.L01-rivalry-excludability-four-types-goods.md) | Public Goods and Common Resources | 5 |
| [M12](modules/module-12/M12.L01-comparative-advantage-revisited-free-trade.md) | International Trade and Synthesis | 5 |
| [M13](modules/module-13/M13.L01-budget-constraints.md) | Budget Constraints, Preferences, and Utility | 5 |
| [M14](modules/module-14/M14.L01-optimal-consumer-choice.md) | Consumer Choice and Demand | 5 |
| [M15](modules/module-15/M15.L01-slutsky-equation.md) | Comparative Statics and Demand Theory | 5 |
| [M16](modules/module-16/M16.L01-intertemporal-choice.md) | Applications of Consumer Theory | 5 |
| [M17](modules/module-17/M17.L01-edgeworth-box-endowments.md) | Exchange Economy and General Equilibrium | 5 |
| [M18](modules/module-18/M18.L01-technology-production-sets.md) | Technology, Production, and Profit Maximisation | 5 |
| [M19](modules/module-19/M19.L01-cost-functions-short-long-run.md) | Costs, Competitive Supply, and Industry Equilibrium | 5 |
| [M20](modules/module-20/M20.L01-monopoly-formal-welfare-loss.md) | Monopoly and Game Theory (Advanced) | 6 |
| [M21](modules/module-21/M21.L01-adverse-selection-lemons.md) | Information Asymmetry and Synthesis | 5 |
| [📝 Quizzes](quizzes/) | 315 practice questions across all 12 introductory modules — multiple choice, calculation, and short answer | 12 modules |
| [🃏 Flashcards](flashcards.md) | 315 interactive flashcards — tap to flip, filter by module or question type, works on any device | All modules |


---

## 🎓 Ask a Question

<!-- Economics AI Chat Widget -->
<div id="econ-chat-widget" style="
  margin: 2rem 0;
  background: white;
  border: 1px solid #e2e8f0;
  border-radius: 12px;
  padding: 1.5rem;
  box-shadow: 0 2px 8px rgba(0,0,0,0.06);
">
  <h3 style="margin:0 0 0.5rem 0; font-size:1rem; color:#2d3748;">🎓 Ask a Question</h3>
  <p style="margin:0 0 1rem 0; font-size:0.85rem; color:#718096;">Ask anything about the course content — concepts, calculations, Australian examples.</p>
  <div style="display:flex; gap:0.5rem;">
    <input id="econ-chat-input" type="text"
      placeholder="e.g. What is the IS-LM model used for?"
      style="flex:1; padding:0.6rem 0.9rem; border:1px solid #cbd5e0; border-radius:8px; font-size:0.9rem; outline:none;"
      onkeydown="if(event.key==='Enter') econAsk()"
    />
    <button onclick="econAsk()" id="econ-chat-btn" style="
      padding:0.6rem 1.2rem; background:#5c6bc0; color:white;
      border:none; border-radius:8px; cursor:pointer; font-size:0.9rem; font-weight:600;
      white-space:nowrap;
    ">Ask →</button>
  </div>
  <div id="econ-chat-response" style="
    margin-top:1rem; padding:1rem; background:#f7fafc;
    border-radius:8px; font-size:0.9rem; line-height:1.6;
    color:#2d3748; display:none;
  "></div>
</div>
<script>
async function econAsk() {
  const input = document.getElementById('econ-chat-input');
  const btn = document.getElementById('econ-chat-btn');
  const resp = document.getElementById('econ-chat-response');
  const q = input.value.trim();
  if (!q) return;
  btn.textContent = '...'; btn.disabled = true;
  resp.style.display = 'block';
  resp.textContent = 'Thinking...';
  try {
    const r = await fetch('https://econ-chat.dgg5dknmth.workers.dev', {
      method: 'POST',
      headers: {'Content-Type':'application/json'},
      body: JSON.stringify({question: q})
    });
    const d = await r.json();
    resp.innerHTML = d.answer.replace(/\n/g,'<br>');
  } catch(e) {
    resp.textContent = 'Error: could not reach the AI. Please try again.';
  }
  btn.textContent = 'Ask →'; btn.disabled = false;
}
</script>
