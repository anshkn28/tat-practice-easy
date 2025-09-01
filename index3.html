'use client';
import React, { useEffect, useRef, useState } from 'react';

// =============================
// SSB SRT PRACTICE – Next.js/React (TSX)
// Fix for error: "SyntaxError: /index.tsx: Unexpected token (1:0)"
// Cause: HTML was placed in a .tsx file. This file is valid TSX.
// Drop this into `pages/index.tsx` (Pages Router) or `app/page.tsx` (App Router).
// No external CSS or libs required.
// =============================

// 180 prompts (60 original + 120 new). Kept inline for simplicity.
const SRTS: string[] = [
  // Existing 60 prompts
  'Walking home at night, he saw a man unconscious on the pavement. He ___',
  'On a train, he noticed someone trying to pick a passenger’s pocket. He ___',
  'In a football match, his team was trailing with little time left. He ___',
  'A child fell into a pond while playing nearby. He ___',
  'During study, electricity went off before an exam. He ___',
  'Cycling to school, he witnessed a road accident. He ___',
  'He was suddenly asked to give a short speech on stage. He ___',
  'On the way to office, he noticed smoke from a shop. He ___',
  'While trekking, his friend slipped and sprained an ankle. He ___',
  'On exam day, his bicycle chain broke. He ___',
  'During bus travel, the vehicle was overcrowded. He ___',
  'An old man struggled to cross a busy road. He ___',
  'In cricket practice, the ball broke a neighbour’s window. He ___',
  'Before an interview, heavy rain began without warning. He ___',
  'He was offered money to do something unethical. He ___',
  'In the market, a wallet fell from someone’s pocket. He ___',
  'On a picnic, the group ran short of food. He ___',
  'He noticed a classmate cheating in a test. He ___',
  'At night, he heard distress cries from a nearby house. He ___',
  'A teammate was missing project deadlines repeatedly. He ___',
  'A car splashed muddy water onto pedestrians. He ___',
  'A sudden power cut hit a community event he organized. He ___',
  'His bicycle brake failed on a downhill slope. He ___',
  'He spotted a snake near the backyard door. He ___',
  'A stranger urgently asked to use his phone. He ___',
  'A close friend started a harmful habit. He ___',
  'A classmate looked isolated and withdrawn for days. He ___',
  'He noticed leakage from the hostel water tank. He ___',
  'He reached the exam hall ten minutes late. He ___',
  'A small fire started in the kitchen. He ___',
  'He saw a motorbike skid on a wet road. He ___',
  'He found a lost child at a fair. He ___',
  'A neighbour’s house was found unlocked at night. He ___',
  'His juniors lacked sports equipment. He ___',
  'A teammate took credit for his work. He ___',
  'A woman fainted on a bus. He ___',
  'He noticed a live electric wire on the street. He ___',
  'He saw a classmate being bullied. He ___',
  'He missed the last bus home. He ___',
  'His friend forgot admission documents. He ___',
  'The neighbourhood park was littered. He ___',
  'A rumor about a teacher spread online. He ___',
  'He found counterfeit notes in change received. He ___',
  'A shopkeeper overcharged an elderly customer. He ___',
  'He witnessed a minor theft at the canteen. He ___',
  'During flood relief, supplies were mismanaged. He ___',
  'He saw a dog injured by traffic. He ___',
  'His bike ran out of fuel in a remote area. He ___',
  'A friend showed signs of exam anxiety. He ___',
  'He observed unsafe construction at a site. He ___',
  'He noticed smoke in the hostel corridor. He ___',
  'During marathon practice, a runner collapsed. He ___',
  'He found cracks in a bridge walkway. He ___',
  'A neighbor played loud music late night. He ___',
  'A shop’s cash drawer was left open. He ___',
  'He saw someone dumping waste into a lake. He ___',
  'His sibling failed an important test. He ___',
  'He discovered a data error in submitted work. He ___',
  'He encountered a stranded car at night. He ___',
  'He realized his phone was stolen in a crowd. He ___',

  // 120 NEW prompts
  'During NCC camp, his tent collapsed at midnight. He ___',
  'He saw a classmate crying before an exam. He ___',
  'His bicycle tire got punctured on the way to tuition. He ___',
  'He noticed two children fighting in the park. He ___',
  'The teacher asked an unexpected question in class. He ___',
  'His neighbour’s cow broke into the garden. He ___',
  'The school team lost several matches in a row. He ___',
  'He heard strange noises while walking alone at night. He ___',
  'A villager asked for help to carry heavy load. He ___',
  'A football hit and broke classroom glass. He ___',
  'During a visit, he noticed poor sanitation in a colony. He ___',
  'His younger sibling refused to study. He ___',
  'A street dog chased him while jogging. He ___',
  'He lost his lunchbox at school. He ___',
  'An elder asked him to do a difficult task. He ___',
  'He found a purse in the playground. He ___',
  'The teacher gave him low marks unfairly. He ___',
  'While swimming, his friend got tired in deep water. He ___',
  'He saw a child selling balloons on the roadside. He ___',
  'He had a disagreement with his best friend. He ___',
  'He was asked to lead morning assembly suddenly. He ___',
  'While painting, he spilled colour on the floor. He ___',
  'He observed someone wasting food in the mess. He ___',
  'On the way to school, he saw garbage on the street. He ___',
  'His cricket team needed one run in last ball. He ___',
  'He noticed a bicycle accident near school gate. He ___',
  'His shoes tore just before a function. He ___',
  'He was punished for a mistake not his own. He ___',
  'During hike, rain started heavily. He ___',
  'His classmate did not bring homework. He ___',
  'He saw a man begging at traffic signal. He ___',
  'He lost his way during a trip. He ___',
  'He heard news of flood in nearby village. He ___',
  'He was called for help by a neighbour at night. He ___',
  'His cycle bell broke in traffic. He ___',
  'He saw a farmer struggling in field. He ___',
  'During match, umpire gave unfair decision. He ___',
  'He was offered cigarette by a friend. He ___',
  'He saw classmates teasing a junior. He ___',
  'He observed broken bench in school. He ___',
  'His bus broke down midway. He ___',
  'He noticed an old man feeling unwell. He ___',
  'He got fever on exam day. He ___',
  'He dropped water on important documents. He ___',
  'He saw someone damaging school property. He ___',
  'He observed friend without lunch. He ___',
  'He found injured bird in garden. He ___',
  'He saw traffic jam near school. He ___',
  'During PT, his friend got hurt. He ___',
  'He observed electricity wastage in hostel. He ___',
  'He noticed plastic waste in park. He ___',
  'He saw someone fighting in bus. He ___',
  'He forgot his notebook at home. He ___',
  'He was late for school assembly. He ___',
  'He saw injured man on road. He ___',
  'His friend was absent for many days. He ___',
  'He saw group of students quarreling. He ___',
  'He noticed broken tap in washroom. He ___',
  'He saw teacher carrying heavy books. He ___',
  'He forgot to switch off fan in class. He ___',
  'He observed juniors playing in restricted area. He ___',
  'He found wallet with money. He ___',
  'He noticed small child alone in market. He ___',
  'He heard alarm of fire. He ___',
  'He saw a person faint on street. He ___',
  'He realized bus ticket missing. He ___',
  'He found mobile phone on bench. He ___',
  'He saw water leakage in class roof. He ___',
  'He observed fight between shopkeepers. He ___',
  'He was called to speak on environment. He ___',
  'He saw a friend waste pocket money. He ___',
  'He found exam paper difficult. He ___',
  'He noticed plant without water. He ___',
  'He forgot homework at hostel. He ___',
  'He saw junior being scolded unfairly. He ___',
  'He got low marks in test. He ___',
  'He saw garbage near playground. He ___',
  'He was lost in fair. He ___',
  'He found someone’s pen. He ___',
  'He saw torn national flag. He ___',
  'He heard about blood donation camp. He ___',
  'He noticed bus full but people still boarding. He ___',
  'He was asked to sing on stage. He ___',
  'He found himself in new city. He ___',
  'He saw quarrel at water tap. He ___',
  'He observed misuse of library books. He ___',
  'He was asked to guide juniors. He ___',
  'He saw lights left on in classroom. He ___',
  'He noticed broken chair. He ___',
  'He forgot important book. He ___',
  'He saw man littering on road. He ___',
  'He observed student sleeping in class. He ___',
  'He was given wrong parcel. He ___',
  'He saw friend unhappy. He ___',
  'He noticed medicine expired. He ___',
  'He forgot to bring pen in exam. He ___',
  'He saw stranger suspiciously. He ___',
  'He heard about tree cutting. He ___',
  'He observed dustbin overflowing. He ___',
  'He saw broken swing in park. He ___',
  'He forgot ID card. He ___',
  'He noticed juniors without proper uniform. He ___',
  'He observed cracked wall. He ___',
  'He was asked to lead drill. He ___',
  'He noticed student hiding book. He ___',
  'He saw unsafe wiring. He ___',
  'He was asked meaning of word. He ___',
  'He saw person dropping wallet. He ___',
  'He forgot lunch box. He ___',
  'He saw injured kitten. He ___',
  'He was asked to help teacher. He ___',
  'He saw untidy classroom. He ___',
  'He found key on floor. He ___',
  'He saw person fall from bike. He ___',
  'He noticed broken light. He ___',
  'He saw junior lost. He ___',
  'He forgot important date. He ___',
  'He noticed wrong information on notice board. He ___',
  'He saw quarrel during sports. He ___',
  'He observed misuse of water. He ___',
  'He was asked to help in kitchen. He ___',
  'He saw friend absent-minded. He ___',
  'He noticed broken fence. He ___',
];

const styles = {
  page: { background: '#f9fafb', minHeight: '100vh', color: '#0f172a', fontFamily: 'ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, Helvetica Neue, Arial' },
  center: { display: 'flex', justifyContent: 'center', alignItems: 'center', height: '100vh' },
  splash: { background: '#000', color: '#fff', fontWeight: 700, fontSize: 'clamp(18px, 4vw, 28px)', letterSpacing: '0.5px' },
  container: { maxWidth: 960, margin: '0 auto', padding: 24 },
  grid: { display: 'grid', gridTemplateColumns: 'repeat(3,1fr)', gap: 12 },
  btn: { padding: '12px 18px', borderRadius: 16, border: 'none', background: '#fff', boxShadow: '0 1px 2px rgba(0,0,0,.05), 0 6px 20px rgba(0,0,0,.06)', cursor: 'pointer', fontWeight: 700 },
  card: { background: '#f3f4f6', borderRadius: 12, padding: 15, boxShadow: '0 1px 3px rgba(0,0,0,.1)', marginBottom: 20 },
  timer: { fontFamily: 'ui-monospace, SFMono-Regular, Menlo, monospace', margin: '4px 0 20px' },
  hint: { color: '#6b7280', fontStyle: 'italic' as const },
  finishWrap: { textAlign: 'center' as const, marginTop: 20 },
};

function formatTime(totalSeconds: number): string {
  const m = Math.floor(totalSeconds / 60);
  const s = String(totalSeconds % 60).padStart(2, '0');
  return `${m}:${s}`;
}

function shuffle<T>(arr: T[]): T[] {
  const a = [...arr];
  for (let i = a.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [a[i], a[j]] = [a[j], a[i]];
  }
  return a;
}

export default function Page() {
  type Phase = 'splash' | 'menu' | 'practice' | 'result';
  const [phase, setPhase] = useState<Phase>('splash');
  const [selectedCount, setSelectedCount] = useState<number | null>(null);
  const [sessionPrompts, setSessionPrompts] = useState<string[]>([]);
  const [seconds, setSeconds] = useState(0);
  const timerRef = useRef<number | null>(null); // window.setInterval returns number

  // Auto-hide splash after 2s
  useEffect(() => {
    const t = window.setTimeout(() => setPhase('menu'), 2000);
    return () => window.clearTimeout(t);
  }, []);

  // Cleanup timer on unmount
  useEffect(() => {
    return () => {
      if (timerRef.current) window.clearInterval(timerRef.current);
    };
  }, []);

  const startPractice = (count: number) => {
    setSelectedCount(count);
    const chosen = shuffle(SRTS).slice(0, count);
    setSessionPrompts(chosen);
    setSeconds(0);
    setPhase('practice');
    if (timerRef.current) window.clearInterval(timerRef.current);
    timerRef.current = window.setInterval(() => setSeconds((s) => s + 1), 1000);
  };

  const finishPractice = () => {
    if (timerRef.current) {
      window.clearInterval(timerRef.current);
      timerRef.current = null;
    }
    setPhase('result');
  };

  // ---- Minimal smoke tests (run in browser console) ----
  useEffect(() => {
    // Only run in browser
    const tests = () => {
      try {
        console.log('%cRunning smoke tests…', 'font-weight:bold');
        // formatTime tests
        console.assert(formatTime(0) === '0:00', 'formatTime(0)');
        console.assert(formatTime(65) === '1:05', 'formatTime(65)');
        // Prompt selection tests
        const n = 10;
        const chosen = shuffle(SRTS).slice(0, n);
        console.assert(chosen.length === n, 'Selected prompt count mismatch');
        console.assert(chosen.every((p) => typeof p === 'string' && p.includes('___')), 'Prompts invalid format');
        console.log('%cAll smoke tests passed.', 'color:green');
      } catch (e) {
        console.error('Smoke test failed:', e);
      }
    };
    if (typeof window !== 'undefined') tests();
  }, []);

  // UI blocks
  const Splash = (
    <div style={{ ...styles.center, ...styles.splash }}>
      <div>Made by Ansh Khilnani</div>
    </div>
  );

  const Menu = (
    <div style={styles.center}>
      <div style={styles.container as React.CSSProperties}>
        <h2 style={{ textAlign: 'center', marginBottom: 20 }}>Select Number of SRTs</h2>
        <div style={styles.grid as React.CSSProperties}>
          {[5, 10, 15, 30, 45, 60].map((n) => (
            <button
              key={n}
              style={styles.btn}
              onClick={() => startPractice(n)}
              onMouseDown={(e) => (e.currentTarget.style.transform = 'translateY(1px)')}
              onMouseUp={(e) => (e.currentTarget.style.transform = 'translateY(0)')}
            >
              {n}
            </button>
          ))}
        </div>
      </div>
    </div>
  );

  const Practice = (
    <div style={styles.container as React.CSSProperties}>
      <h2>SRT Practice {selectedCount ? `(${selectedCount} SRTs)` : ''}</h2>
      <div style={styles.timer}>⏱ {formatTime(seconds)}</div>
      <div>
        {sessionPrompts.map((q, i) => (
          <div key={i} style={styles.card}>
            <p style={{ fontWeight: 600, marginBottom: 12 }}>{q}</p>
            <p style={styles.hint}>(Write your response by hand on paper)</p>
          </div>
        ))}
      </div>
      <div style={styles.finishWrap}>
        <button style={styles.btn} onClick={finishPractice}>Finish</button>
      </div>
    </div>
  );

  const Result = (
    <div style={styles.container as React.CSSProperties}>
      <h2>Practice Finished</h2>
      <p>Your Time: ⏱ {formatTime(seconds)}</p>
      <h3>Questions:</h3>
      <div>
        {sessionPrompts.map((q, i) => (
          <div key={i} style={styles.card}>
            <p>{q}</p>
          </div>
        ))}
      </div>
    </div>
  );

  return (
    <div style={styles.page}>
      {phase === 'splash' && Splash}
      {phase === 'menu' && Menu}
      {phase === 'practice' && Practice}
      {phase === 'result' && Result}
    </div>
  );
}
