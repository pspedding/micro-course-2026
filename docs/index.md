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

<!-- Economics AI Chat Widget — P1: adaptive-tutor (feature branch only) -->
<!-- CDN: DOMPurify (XSS sanitisation) + marked (markdown rendering) -->
<script src="https://cdn.jsdelivr.net/npm/dompurify@3/dist/purify.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/marked@12/marked.min.js"></script>

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

  <!-- Mode toggle -->
  <div style="display:flex;gap:0.5rem;margin-bottom:0.8rem;">
    <button class="econ-mode-btn" data-mode="explain"
      style="padding:0.3rem 0.8rem;border:1px solid #9fa8da;border-radius:6px;cursor:pointer;font-size:0.82rem;background:#5c6bc0;color:white;">
      Explain
    </button>
    <button class="econ-mode-btn" data-mode="tutor"
      style="padding:0.3rem 0.8rem;border:1px solid #9fa8da;border-radius:6px;cursor:pointer;font-size:0.82rem;background:#e8eaf6;color:#3949ab;">
      Tutor
    </button>
  </div>

  <!-- Conversation thread -->
  <div id="econ-chat-thread" style="max-height:380px;overflow-y:auto;margin-bottom:0.8rem;display:flex;flex-direction:column;gap:0.3rem;"></div>

  <!-- Input row -->
  <div style="display:flex; gap:0.5rem;">
    <input id="econ-chat-input" type="text"
      placeholder="e.g. What is the IS-LM model used for?"
      style="flex:1; padding:0.6rem 0.9rem; border:1px solid #cbd5e0; border-radius:8px; font-size:0.9rem; outline:none;"
    />
    <button onclick="econAsk()" id="econ-chat-btn" style="
      padding:0.6rem 1.2rem; background:#5c6bc0; color:white;
      border:none; border-radius:8px; cursor:pointer; font-size:0.9rem; font-weight:600;
      white-space:nowrap;
    ">Ask →</button>
    <button id="econ-chat-clear" type="button" style="
      padding:0.6rem 0.8rem; background:#e8eaf6; color:#3949ab;
      border:1px solid #9fa8da; border-radius:8px; cursor:pointer; font-size:0.9rem;
    ">Clear</button>
  </div>

  <div id="econ-chat-response" style="
    margin-top:1rem; padding:1rem; background:#f7fafc;
    border-radius:8px; font-size:0.9rem; line-height:1.6;
    color:#2d3748; display:none;
  "></div>
</div>

<script>
(function(){
  // STAGING: points at staging Worker — swap to production URL after tests pass
  var WORKER='https://econ-chat-staging.dgg5dknmth.workers.dev';
  // PRODUCTION (do not activate until staging tests pass):
  // var WORKER='https://econ-chat.dgg5dknmth.workers.dev';

  var MAX_TURNS=10, MAX_Q=4000;
  var history=[], mode='explain';

  function estimateTokens(s){ return Math.ceil((s||'').length/4); }

  function trimHistory(h){
    var msgs=h.slice();
    while(msgs.length>1 && msgs.reduce(function(s,m){return s+estimateTokens(m.content);},0)>4000)
      msgs.splice(0,2);
    return msgs.slice(-(MAX_TURNS*2));
  }

  function detectContext(){
    var p=window.location.pathname;
    var cm=p.match(/macro-course|micro-course|econ-course/);
    var mm=p.match(/module-([0-9]+)/i);
    var lm=p.match(/(M[0-9]{2}[-.]L[0-9]{2}[^/]*)/i);
    return {
      course: cm ? cm[0].replace(/-course(-[0-9]+)?/,'') : null,
      module: mm ? 'M'+(mm[1].length<2?'0':'')+mm[1] : null,
      lesson: lm ? lm[1] : null
    };
  }

  function getWeakModules(){
    try{
      var keys=Object.keys(localStorage).filter(function(k){return k.indexOf('macro-')===0&&k.slice(-3)==='-v1';});
      for(var i=0;i<keys.length;i++){
        var s=JSON.parse(localStorage.getItem(keys[i])||'{}');
        var w=Object.keys(s.mastery||{}).filter(function(k){
          var v=s.mastery[k];
          return v.attempts>=3&&v.correct/v.attempts<0.65;
        }).slice(0,5);
        if(w.length) return w;
      }
    }catch(e){}
    return [];
  }

  function renderSafe(el,text){
    var html=marked.parse(text);
    el.innerHTML=DOMPurify.sanitize(html,{USE_PROFILES:{html:true}});
    if(window.MathJax&&MathJax.typesetPromise) MathJax.typesetPromise([el]).catch(function(){});
  }

  function appendThread(role,text){
    var t=document.getElementById('econ-chat-thread');
    if(!t) return;
    var d=document.createElement('div');
    d.style.cssText=role==='user'
      ?'padding:0.55rem 0.8rem;background:#eef2ff;border-radius:8px;font-size:0.9rem;margin-bottom:0.2rem;'
      :'padding:0.55rem 0.8rem;background:#f7fafc;border-radius:8px;font-size:0.9rem;line-height:1.65;margin-bottom:0.2rem;';
    if(role==='user') d.textContent=text;
    else renderSafe(d,text);
    t.appendChild(d);
    t.scrollTop=t.scrollHeight;
  }

  function econAsk(){
    var input=document.getElementById('econ-chat-input');
    var btn=document.getElementById('econ-chat-btn');
    var resp=document.getElementById('econ-chat-response');
    var q=(input&&input.value||'').trim();
    if(!q) return;
    if(q.length>MAX_Q){
      if(resp){resp.style.display='block';resp.textContent='Question too long (max 4,000 characters).';}
      return;
    }
    if(btn){btn.textContent='...';btn.disabled=true;}
    if(resp) resp.style.display='none';
    appendThread('user',q);
    if(input) input.value='';

    var ctx=detectContext();
    ctx.weakModules=getWeakModules();
    var payload={question:q,mode:mode,messages:trimHistory(history),context:ctx};

    fetch(WORKER,{method:'POST',headers:{'Content-Type':'application/json'},body:JSON.stringify(payload)})
      .then(function(r){return r.json();})
      .then(function(d){
        if(d.error) throw new Error(d.error);
        history.push({role:'user',content:q},{role:'assistant',content:d.answer});
        if(history.length>MAX_TURNS*2) history.splice(0,2);
        appendThread('assistant',d.answer);
      })
      .catch(function(e){
        if(resp){resp.style.display='block';resp.textContent=e.message||'Error: could not reach the AI. Please try again.';}
      })
      .finally(function(){
        if(btn){btn.textContent='Ask →';btn.disabled=false;}
        if(input) input.focus();
      });
  }

  function clearConversation(){
    history=[];
    var t=document.getElementById('econ-chat-thread');
    if(t) t.innerHTML='';
    var r=document.getElementById('econ-chat-response');
    if(r) r.style.display='none';
  }

  function setMode(m){
    mode=m;
    var btns=document.querySelectorAll('.econ-mode-btn');
    for(var i=0;i<btns.length;i++){
      btns[i].style.background=btns[i].getAttribute('data-mode')===m?'#5c6bc0':'#e8eaf6';
      btns[i].style.color=btns[i].getAttribute('data-mode')===m?'white':'#3949ab';
    }
  }

  function init(){
    var inp=document.getElementById('econ-chat-input');
    if(inp) inp.addEventListener('keydown',function(e){if(e.key==='Enter')econAsk();});
    var btn=document.getElementById('econ-chat-btn');
    if(btn) btn.addEventListener('click',econAsk);
    var clr=document.getElementById('econ-chat-clear');
    if(clr) clr.addEventListener('click',clearConversation);
    var mbtns=document.querySelectorAll('.econ-mode-btn');
    for(var i=0;i<mbtns.length;i++){
      (function(b){b.addEventListener('click',function(){setMode(b.getAttribute('data-mode'));});})(mbtns[i]);
    }
    setMode('explain');
  }

  if(document.readyState==='loading') document.addEventListener('DOMContentLoaded',init);
  else init();

  window.econAsk=econAsk;
})();
</script>
