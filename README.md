
``` // date ranges

### function App() {

### function getDaysBetweenDates(date1, date2) {
    // Convert both dates to milliseconds
    const date1InMs = date1.getTime();
    const date2InMs = date2.getTime();

    // Calculate the difference in milliseconds
    const diffInMs = Math.abs(date1InMs - date2InMs);

    // Convert the difference in milliseconds to days
    const diffInDays = Math.ceil(diffInMs / (1000 * 3600 * 24));

    return diffInDays;
  }

  const date1 = new Date("02/27/2024");
  const date2 = new Date("03/06/2024");
  const daysBetween = getDaysBetweenDates(date1, date2);

  console.log(daysBetween);
  return <div></div>;
}

### export default App;
