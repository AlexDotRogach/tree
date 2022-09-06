# tree
const size = 7;

for (let i = 0; i < size; i++) {
  if (i === 0) {
    console.log(`${createSpace(size)}*`);
    continue;
  }

  console.log(createSpace(size - i) + createSymbol(i * 2));
}

function createSymbol(quantity) {
  let amount = "";

  for (let i = 0; i < quantity; i += 1) {
    amount += "*";
  }

  return amount;
}

function createSpace(quantity) {
  let amount = "";

  for (let i = 0; i < quantity; i += 1) {
    amount += " ";
  }

  return amount;
}
