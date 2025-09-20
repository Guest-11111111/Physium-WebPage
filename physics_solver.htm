# Web Physics Solver

A simple kinematics solver to find the missing variables in uniformly accelerated motion.

**Instructions:**
1.  Enter exactly three of the five variables.
2.  Leave the two unknown variables blank.
3.  Click "Solve" to see the results.

<style>
  body { font-family: sans-serif; }
  .solver-container {
    background-color: #f0f0f0;
    padding: 20px;
    border-radius: 8px;
    max-width: 400px;
  }
  .input-group {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
  }
  .input-group label {
    flex: 1;
  }
  .input-group input {
    flex: 2;
    padding: 5px;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  #solve-button {
    background-color: #4CAF50;
    color: white;
    padding: 10px 15px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
  #solve-button:hover {
    background-color: #45a049;
  }
  #results {
    margin-top: 20px;
    font-weight: bold;
  }
</style>

<div class="solver-container">
  <div class="input-group">
    <label for="s">Displacement (s):</label>
    <input type="number" id="s" placeholder="meters">
  </div>
  <div class="input-group">
    <label for="u">Initial Velocity (u):</label>
    <input type="number" id="u" placeholder="m/s">
  </div>
  <div class="input-group">
    <label for="v">Final Velocity (v):</label>
    <input type="number" id="v" placeholder="m/s">
  </div>
  <div class="input-group">
    <label for="a">Acceleration (a):</label>
    <input type="number" id="a" placeholder="m/s²">
  </div>
  <div class="input-group">
    <label for="t">Time (t):</label>
    <input type="number" id="t" placeholder="seconds">
  </div>
  <button id="solve-button">Solve</button>
  <div id="results"></div>
</div>

<script>
  document.getElementById('solve-button').addEventListener('click', () => {
    const s_in = document.getElementById('s');
    const u_in = document.getElementById('u');
    const v_in = document.getElementById('v');
    const a_in = document.getElementById('a');
    const t_in = document.getElementById('t');
    const resultsDiv = document.getElementById('results');

    const s = s_in.value !== '' ? parseFloat(s_in.value) : null;
    const u = u_in.value !== '' ? parseFloat(u_in.value) : null;
    const v = v_in.value !== '' ? parseFloat(v_in.value) : null;
    const a = a_in.value !== '' ? parseFloat(a_in.value) : null;
    const t = t_in.value !== '' ? parseFloat(t_in.value) : null;

    const values = { s, u, v, a, t };
    const knowns = Object.values(values).filter(val => val !== null).length;

    if (knowns !== 3) {
      resultsDiv.innerHTML = "Error: Please provide exactly three values.";
      return;
    }

    let result_s = s, result_u = u, result_v = v, result_a = a, result_t = t;

    if (u !== null && v !== null && a !== null) { // solve for s, t
      result_t = (v - u) / a;
      result_s = u * result_t + 0.5 * a * result_t * result_t;
    } else if (u !== null && v !== null && t !== null) { // solve for s, a
      result_s = ((u + v) / 2) * t;
      result_a = (v - u) / t;
    } else if (u !== null && v !== null && s !== null) { // solve for a, t
      result_a = (v * v - u * u) / (2 * s);
      result_t = (v - u) / result_a;
    } else if (u !== null && a !== null && t !== null) { // solve for s, v
      result_s = u * t + 0.5 * a * t * t;
      result_v = u + a * t;
    } else if (u !== null && a !== null && s !== null) { // solve for v, t
      result_v = Math.sqrt(u * u + 2 * a * s);
      result_t = (result_v - u) / a;
    } else if (u !== null && t !== null && s !== null) { // solve for v, a
      result_v = (2 * s) / t - u;
      result_a = (result_v - u) / t;
    } else if (v !== null && a !== null && t !== null) { // solve for u, s
      result_u = v - a * t;
      result_s = v * t - 0.5 * a * t * t;
    } else if (v !== null && a !== null && s !== null) { // solve for u, t
      result_u = Math.sqrt(v * v - 2 * a * s);
      result_t = (v - result_u) / a;
    } else if (v !== null && t !== null && s !== null) { // solve for u, a
      result_u = (2 * s) / t - v;
      result_a = (v - result_u) / t;
    } else if (a !== null && t !== null && s !== null) { // solve for u, v
      result_u = (s - 0.5 * a * t * t) / t;
      result_v = result_u + a * t;
    } else {
      resultsDiv.innerHTML = "Could not solve with the given inputs.";
      return;
    }

    resultsDiv.innerHTML = `
      <p>Displacement (s): ${result_s.toFixed(4)} m</p>
      <p>Initial Velocity (u): ${result_u.toFixed(4)} m/s</p>
      <p>Final Velocity (v): ${result_v.toFixed(4)} m/s</p>
      <p>Acceleration (a): ${result_a.toFixed(4)} m/s²</p>
      <p>Time (t): ${result_t.toFixed(4)} s</p>
    `;
  });
</script>
